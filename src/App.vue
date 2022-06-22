<script lang="ts" setup>
import { ref } from 'vue'

const menu = ref({
  left: [
    // 顶部左侧菜单按钮
  ],
  center: [
    // 顶部中间菜单按钮
  ],
  right: [
    // 顶部右侧菜单按钮
  ]
})

const data = ref({
  // 初始化页面数据
})

const runtimeUrl: string = '/runtime/vue3/playground.html'

const propsConfigs: any[] = [
  // 组件属性列表
]

const propsValues: any[] = [
  // 组件默认值
]

const componentGroupList = ref([
  // 组件列表
])
</script>

<template>
  <m-editor
    v-model="data"
    :menu="menu"
    :runtime-url="runtimeUrl"
    :props-configs="propsConfigs"
    :props-values="propsValues"
    :component-group-list="componentGroupList"
  ></m-editor>
</template>

<style>
#app {
  width: 100%;
  height: 100%;
  display: flex;
}
.m-editor {
  flex: 1;
  height: 100%;
}
</style>
