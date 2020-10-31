<template>
  <div id="app">
    <div class="sidebar bg-dark">
      <div class="header">
<!--        <b-avatar size="lg" class="prof"></b-avatar>-->
        <h3 class="prof" style="color: white">Chat Party</h3>
      </div>
      <Nav />
    </div>
    <div class="main">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Nav from './components/Nav'
export default {
  name: "App",
  components: {
    Nav
  }
}
</script>
<style scoped>
*, body{
  margin: 0;
  padding: 0;
}

#app {
  width: 100%;
  height: 100vh;
  display: flex;
}

.sidebar{
  flex: 0.15;
  /*display: flex;*/
  /*border-right: 1px solid silver;*/
}

.header {
  display: flex;
  height: 100px;
}

.prof {
  margin: auto;
}

.main {
  flex: 1;
  /*background: white;*/
}

@media only screen and (max-width: 900px) {
  /*.sidebar {*/
  /*  flex: 0;*/
  /*}*/
}

</style>
