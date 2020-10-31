<template>
  <div class="root">
    <b-nav pills justified vertical class="navigation">
      <b-nav-item to="/" exact exact-active-class="active">
        <b-icon icon="chat-text-fill"></b-icon>
        <span class="hide-on-mobile pl-1">Chats</span>
      </b-nav-item>
      <b-nav-item to="/explore" exact exact-active-class="active">
        <b-icon icon="search"></b-icon>
        <span class="hide-on-mobile pl-1">Search</span>
      </b-nav-item>
      <b-nav-item to="/friends" exact exact-active-class="active">
        <b-icon icon="people-fill"></b-icon>
        <span class="hide-on-mobile pl-1">Friends</span>
      </b-nav-item>
      <b-nav-item to="/about" exact exact-active-class="active">
        <b-icon icon="gear-fill"></b-icon>
        <span class="hide-on-mobile pl-1">Settings</span>
      </b-nav-item>
    </b-nav>
  </div>
</template>

<script>
export default {
  name: "Nav",
  components:{

  }
}
</script>

<style scoped>

@media only screen and (max-width: 900px) {
  .hide-on-mobile {
    display: none;
  }
}
</style>