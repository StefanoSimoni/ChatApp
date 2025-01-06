<template>
  <div class="messageItem">
    <img src="/avatars/avatar-02.jpg" alt="John Diego" />
    <div class="data">
      <div class="userData">
        <h1>John Diego</h1>
        <span>14:45:11</span>
      </div>
      <p>Hola Mundo!</p>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.messageItem {
  @apply flex gap-3 px-5;
}

img {
  @apply w-12 h-12 rounded-full;
}

.data {
  @apply flex flex-col gap-1;
}

.userData {
  @apply flex gap-2;
}

h1 {
  @apply text-white font-bold;
}

span {
  @apply text-zinc-600;
}

p {
  @apply text-white bg-zinc-800 p-3 rounded-r-2xl rounded-bl-2xl max-w-full break-all;
}
</style>
