<template>
  <main>
    <Aside />
    <RouterView />
  </main>
</template>

<script setup>
import { RouterView } from 'vue-router'
import Aside from '@/components/Aside.vue'
</script>

<style scoped>
main {
  @apply bg-neutral-900 h-screen flex;
}
</style>
