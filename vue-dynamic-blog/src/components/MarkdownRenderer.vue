<template>
  <div v-html="compiledMarkdown"></div>
</template>

<script>
import MarkdownIt from 'markdown-it'

export default {
  name: 'MarkdownRenderer',
  props: {
    content: {
      type: String,
      required: true
    }
  },
  computed: {
    compiledMarkdown() {
      const md = new MarkdownIt({
        html: true,
        linkify: true,
        typographer: true
      })
      return md.render(this.content)
    }
  }
}
</script>

<style scoped>
/* Add your custom styles here if needed */
</style>
