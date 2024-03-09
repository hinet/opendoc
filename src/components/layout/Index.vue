<template>
  <div class="flex flex-row h-full">
    <nav class="flex flex-col w-64 bg-gray-100 h-full">
      <div class="h-10 flex items-center justify-center">
        <a href="#" class="text-2xl font-bold text-gray-900">Menu</a>
      </div>
      <div class="flex-grow">
        <ul class="py-4">
          <li class="mb-2"><a href="#" class="block p-2 rounded hover:bg-gray-200">首页</a></li>
          <li class="mb-2">
            <a href="#" class="block p-2 rounded hover:bg-gray-200">关于我们</a>
          </li>
          <li class="mb-2"><a href="#" class="block p-2 rounded hover:bg-gray-200">服务</a></li>
          <li class="mb-2">
            <a href="#" class="block p-2 rounded hover:bg-gray-200">联系我们</a>
          </li>
        </ul>
      </div>
    </nav>
    <div class="container px-6">
      <slot></slot>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  setup() {
    return {}
  }
})
</script>

<style lang="less" scoped></style>
