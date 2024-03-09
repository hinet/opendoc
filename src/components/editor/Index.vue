<script lang="ts" setup>
import { ref } from 'vue'
import { Editor, Viewer } from '@bytemd/vue-next'
import gfm from '@bytemd/plugin-gfm'
import 'bytemd/dist/index.css'
let content = ref('')

const plugins = [gfm()]

const handleChange = (v: string) => {
  console.log(v)
  content.value = v
}
</script>
<template>
  <Editor :value="content" :plugins="plugins" @change="handleChange" />
</template>
<style lang="less" scoped></style>
