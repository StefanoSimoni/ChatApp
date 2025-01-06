<template>
  <div>
    <input type="text" placeholder="Search" />
    <Icon class="icon" icon="ic:outline-search" />
  </div>
</template>

<script setup></script>

<style scoped>
div {
  @apply relative w-full bg-neutral-900 rounded-lg;
}

input {
  @apply w-11/12 p-1 pl-2 bg-neutral-900 placeholder:text-neutral-200 text-neutral-200 rounded-l-lg outline-none;
}

.icon {
  @apply absolute top-2 right-2 cursor-pointer text-neutral-200;
}
</style>
