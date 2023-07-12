<template>
  <header>
    <h1>我的 ToDoList</h1>
    <input type="text" placeholder="What is your focus today?" />
    <button>Add</button>
  </header>
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
