<script>
import { ref, reactive } from 'vue';
import { QuillEditor } from '@vueup/vue-quill';
import BlotFormatter from 'quill-blot-formatter';
import '@vueup/vue-quill/dist/vue-quill.snow.css';
export default {
    components: {
        QuillEditor,
    },
    setup() {
        const modules = {
            name: 'blotFormatter',
            module: BlotFormatter,
            options: {
                /* options */
            },
        };
        return { modules };
    },
};
</script>

<template>
  <QuillEditor
    theme="snow"
    toolbar="#custom-toolbar"
    :modules="modules"
  >
    <template #toolbar>
      <div id="custom-toolbar">
        <button class="ql-bold"></button>
        <button class="ql-italic"></button>
        <button class="ql-image"></button>

      </div>
    </template>
  </QuillEditor>
</template>

<style>
</style>