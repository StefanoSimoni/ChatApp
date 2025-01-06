<template>
  <div>
    <h1>General</h1>
    <img src="/avatars/avatar-02.jpg" alt="John Diego" />
  </div>
</template>

<script setup></script>

<style scoped>
div {
  @apply flex justify-between items-center sticky top-0 px-5 py-3;
}

h1 {
  @apply text-white text-3xl font-bold;
}

img {
  @apply w-12 h-12 rounded-full border-4 border-zinc-700;
}
</style>
