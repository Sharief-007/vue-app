<template>
<div class="root d-flex align-items-center">
  <div class="image ">
    <b-avatar size="50px" variant="primary"></b-avatar>
  </div>
  <div class="d-flex flex-column pl-2 flex-grow-1">
    <h3 class="m-0" id="recepient-name">Sharief</h3>
    <p>Message mess lorem ipsum</p>
  </div>
  <div class="d-flex flex-grow-1">
    <b-badge variant="primary" style="margin: auto">5</b-badge>
  </div>
</div>
</template>

<script>
export default {
  name: "Recepient"
}
</script>

<style scoped>
.root {
  padding: 0 5px;
  /*border-bottom: 2px solid #edece8;*/
  background-color: #292b2c;
  color: #feefef;
}

.root:hover {
  /*background: #edece8;*/
  background-color: rgba(0,0,0,0.75);
  cursor: pointer;
}

#recepient-name{
  padding-top: 10px;
}
</style>