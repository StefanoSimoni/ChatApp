<template>
  <div class="inputChat">
    <textarea name="message" id="message" autofocus></textarea>
    <Icon class="send" icon="mingcute:send-line" />
  </div>
</template>

<script setup></script>

<style scoped>
.inputChat {
  @apply flex justify-between items-center w-full sticky bottom-0 pl-2 pt-3;
}

textarea {
  @apply w-full resize-none bg-zinc-800 outline-none p-1 text-white rounded-tl-md;
}

.send {
  @apply size-8 cursor-pointer bg-zinc-800 h-full text-white px-1;
}
</style>
