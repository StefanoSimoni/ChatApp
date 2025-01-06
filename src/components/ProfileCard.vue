<template>
  <div class="card">
    <div class="left">
      <img src="/avatars/avatar-02.jpg" alt="John Diego" />
      <div class="userData">
        <h1>John Diego</h1>
        <p :class="isOnline ? 'bg-green-500' : 'bg-red-500'">{{ isActive }}</p>
      </div>
    </div>
    <Icon class="right" icon="ic:baseline-more-vert" @click="router.push('/profile')" />
  </div>
</template>

<script setup>
import router from '@/router'
import { computed, ref } from 'vue'

const isActive = ref('Active')

const isOnline = computed(() => (isActive.value === 'Active' ? true : false))
</script>

<style scoped>
.card {
  @apply w-full flex justify-between bg-zinc-600 p-2 rounded-xl items-center;
}

.left {
  @apply flex gap-3;
}

img {
  @apply w-12 h-12 rounded-lg border-zinc-800 border-2;
}

.userData {
  @apply flex flex-col w-fit justify-between;
}

h1 {
  @apply text-white font-bold;
}

p {
  @apply text-xs w-14 text-center rounded-full text-white;
}

.right {
  @apply text-zinc-400 text-xl cursor-pointer;
}
</style>
