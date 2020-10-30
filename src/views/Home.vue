<template>
  <div id="root">
    <div class="receipints-sidebar d-flex flex-column justify-content-stretch" >
      <Header/>
      <div class="searchbar bg-dark">
        <div class="searchshape">
          <b-icon icon="search"></b-icon>
          <input type="search" class="input-search" placeholder="Search...">
        </div>
      </div>
      <div class="receipints-list">
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
        <Recepient/>
      </div>
    </div>
    <div class="chat-area">

    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header";
import Recepient from "@/components/Recepient";
export default {
  name: 'Home',
  components: {
    Header,
    Recepient
  }
}
</script>

<style scoped>
#root {
  width: 100%;
  height: 100%;
  display: flex;
}

.receipints-sidebar{
  flex: 0.35;
}

.chat-area{
  flex: 1;
}

.searchbar {
  padding: 10px;
}

.searchshape{
  /*color: white;*/
  display: flex;
  align-items: center;
  /*background: white;*/
  background-color: lightgrey;
  padding: 5px;
  border-radius: 20px;
}

.input-search{
  flex: 1;
  outline: none;
  border: none;
  padding: 0 10px;
  background-color: lightgrey;
}

.receipints-list{
  flex: 1;
  overflow: auto;
}
.receipints-list::-webkit-scrollbar {
  width: 8px;
  background-color: #F5F5F5;
}
.receipints-list::-webkit-scrollbar-track {
  -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
  border-radius: 10px;
  /*background-color: #F5F5F5;*/
  background: linear-gradient(to bottom right, #5bc0de, #f7f7f7);
}
.receipints-list::-webkit-scrollbar-thumb {
  border-radius: 10px;
  -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3);
  /*background-color: #D62929;*/
  background: #0275d8;
}
</style>