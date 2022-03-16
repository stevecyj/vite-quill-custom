<script>
import { ref, reactive } from 'vue';
import { QuillEditor } from '@vueup/vue-quill';
import '@vueup/vue-quill/dist/vue-quill.snow.css';
export default {
    components: {
        QuillEditor,
    },
    setup() {
        return {};
    },
};
</script>

<template>
  <QuillEditor
    theme="snow"
    toolbar="#custom-toolbar"
  >
    <template #toolbar>
      <div id="custom-toolbar">
        <button class="ql-bold"></button>

      </div>
    </template>
  </QuillEditor>
</template>

<style>
</style>