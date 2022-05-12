<template>
  <div class="app">
    <Editor :data="state"></Editor>
  </div>
</template>

<script>
import data from './data.json'
import { ref } from '@vue/reactivity'
import Editor from '@/packages/editor.jsx'
export default {
  components:{
    Editor
  },
  setup() {
    const state = ref(data);

    return {
      state
    }
  }
}
</script>

<style lang="scss">

</style>
