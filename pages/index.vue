<template>
  <Editor ref="editor" nativeEmoji :outline="true" :preview="true" v-model="text" />
</template>

<script>
import { Editor } from 'vuetify-markdown-editor';

export default {
  name: 'app',
  components: {
    Editor
  },
  data() {
    return {
      text: ''
    };
  },
  mounted() {
    this.$refs.editor.focus();
  }
};
</script>
