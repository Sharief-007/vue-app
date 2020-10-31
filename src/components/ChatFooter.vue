<template>
<div class="root d-flex align-items-center bg-light p-2">
  <div class="flex-grow-1 mr-2 ml-2">
      <input type="text" placeholder="Type a message..." class="msg-input" autocomplete="off">
  </div>
  <div class="d-flex">
    <b-button variant="primary" >
      <b-icon icon="cursor-fill"></b-icon>
    </b-button>
  </div>
</div>
</template>

<script>
export default {
  name: "ChatFooter"
}
</script>

<style scoped>
.msg-input {
  width: 100%;
  outline: none;
  border:none;
  padding: 5px 15px;
  border-radius: 15px;
  background-color: lightgrey;
}
</style>