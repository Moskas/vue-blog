<template>
  <div>
    <MarkdownRenderer :content="markdownContent" />
  </div>
</template>

<script lang="ts">
import MarkdownRenderer from '../components/MarkdownRenderer.vue'

export default {
  name: 'App',
  components: {
    MarkdownRenderer
  },
  data() {
    return {
      markdownContent:
        '# Hello, Vue 3 and Markdown!\n\nThis is a paragraph with **bold** text and *italic* text.'
    }
  }
}
</script>
