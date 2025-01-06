<template>
  <main>
    <div>
      <span><img src="/avatars/avatar-02.jpg" alt="John Diego" /></span>
      <h1>Username</h1>
      <input type="text" placeholder="John Diego" v-model="username" />
      <button @click="changeUsername">Access</button>
    </div>
  </main>
</template>

<script setup>
import router from '@/router'
import { ref } from 'vue'

const username = ref('')

const changeUsername = () => {
  if (username.value === '') {
    router.go(-1)
  }
}
</script>

<style scoped>
main {
  @apply bg-neutral-900 h-screen flex justify-center items-center;
}

div {
  @apply flex flex-col bg-zinc-800 p-7 rounded-xl gap-2;
}

span {
  @apply flex justify-center;
}

img {
  @apply w-40 h-40 rounded-full border-8 border-zinc-600;
}

h1 {
  @apply text-white text-lg font-medium;
}

input {
  @apply bg-neutral-900 px-4 py-3 rounded-lg w-64;
}

button {
  @apply bg-zinc-600 text-white py-2 rounded-lg font-medium mt-3;
}
</style>
