<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <HelloWorld msg="Hello!" />
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/blog">Blog</RouterLink>
        <RouterLink to="/blog/post">Post</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
