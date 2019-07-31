<template>
  <v-app>
    <Editor ref="editor" nativeEmoji :outline="false" :preview="true" v-model="text" />
  </v-app>
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
