<template>
  <div class="chat d-flex flex-column justify-content-stretch">
    <ChatHeader/>
    <ChatBody class="chat-body"/>
    <ChatFooter/>
  </div>
</template>

<script>
import ChatHeader from "@/components/ChatHeader";
import ChatFooter from "@/components/ChatFooter";
import ChatBody from "@/components/ChatBody";

export default {
  name: "Chat",
  components:{
    ChatHeader,
    ChatFooter,
    ChatBody
  }
}
</script>

<style scoped>
.chat{
  height: 100%;
}
.chat-body {
  flex: 1;
  background-color: white;
}
</style>