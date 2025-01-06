<template>
  <div class="aside">
    <InputSearch />
    <ProfileCard />
    <Channels />
  </div>
</template>

<script setup>
import InputSearch from './InputSearch.vue'
import ProfileCard from './ProfileCard.vue'
import Channels from './Channels.vue'
</script>

<style scoped>
.aside {
  @apply bg-zinc-800 py-4 pl-2 pr-5 flex-1 flex flex-col gap-5;
}
</style>
