<template>
  <footer>
    <input type="checkbox" />
    <label for="">已完成全部</label>
    <div><span>进度：0 / 2</span></div>

    <button>隐藏已完成内容</button>
  </footer>
</template>

<script setup>
import {
  ref,
  reactive,
  toRefs,
  onBeforeMount,
  onMounted,
  watchEffect,
  computed,
} from 'vue'

console.log('1-开始创建组件-setup')
/**
 * 数据部分
 */
const data = reactive({})
onBeforeMount(() => {
  //console.log('2.组件挂载页面之前执行----onBeforeMount')
})
onMounted(() => {
  //console.log('3.-组件挂载到页面之后执行-------onMounted')
})
watchEffect(() => {})
// 使用toRefs解构
// let { } = { ...toRefs(data) }
defineExpose({
  ...toRefs(data),
})
</script>
<style scoped lang="less"></style>
