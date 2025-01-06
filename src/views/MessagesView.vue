<template>
  <div class="messagesView">
    <ChannelHeader />
    <div class="messages">
      <MessageItem />
    </div>
    <InputChat />
  </div>
</template>

<script setup>
import ChannelHeader from '@/components/ChannelHeader.vue'
import MessageItem from '@/components/MessageItem.vue'
import InputChat from '@/components/InputChat.vue'
</script>

<style scoped>
.messagesView {
  @apply flex flex-col h-full flex-[4];
}

.messages {
  @apply overflow-y-scroll h-full;
}
</style>
