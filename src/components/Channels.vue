<template>
  <div class="channels">
    <div class="title">
      <span @click="router.replace({ path: '/' })">
        <h1>Channels</h1>
        <Icon class="hashtag" icon="ic:baseline-tag" />
      </span>
    </div>
    <ChannelItem />
  </div>
</template>

<script setup>
import router from '@/router'
import ChannelItem from './ChannelItem.vue'
</script>

<style scoped>
.channels {
  @apply flex flex-col gap-5 overflow-y-scroll;
}

.title {
  @apply flex items-center px-3;
}

span {
  @apply flex items-center cursor-pointer;
}

h1 {
  @apply text-white font-bold mr-2 text-2xl;
}

.hashtag {
  @apply text-zinc-400 size-6;
}
</style>
