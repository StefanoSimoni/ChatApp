<template>
  <RouterLink to="/1">
    <div>
      <h1>General</h1>
      <p>27</p>
    </div>
  </RouterLink>
</template>

<script setup>
import { RouterLink } from 'vue-router'
</script>

<style scoped>
div {
  @apply flex justify-between items-center cursor-pointer px-3 py-2;
}

div:hover {
  @apply bg-neutral-900 rounded-lg;
}

h1 {
  @apply text-zinc-300 text-lg;
}

p {
  @apply bg-zinc-500 text-white px-3 py-1 rounded-full text-xs font-bold;
}
</style>
