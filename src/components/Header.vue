<template>
<div class="d-flex justify-content-between align-items-center p-2 bg-dark">
  <b-avatar></b-avatar>
  <b-button-toolbar>
    <b-button-group>
      <b-button title="Compose Message" variant="dark">
        <b-icon icon="inbox-fill"></b-icon>
      </b-button>
      <b-dropdown variant="dark" right no-caret>
        <template #button-content>
          <b-icon icon="three-dots-vertical"></b-icon>
        </template>
        <b-dropdown-item>
          <b-icon icon="pencil-square"></b-icon> Compose
        </b-dropdown-item>
        <b-dropdown-divider></b-dropdown-divider>
        <b-dropdown-group id="dropdown-group-1" header="Profile">
          <b-dropdown-item>
            <b-icon icon="person-fill"></b-icon> Profile
          </b-dropdown-item>
          <b-dropdown-item-button>
            <b-icon icon="gear-fill"></b-icon> Settings
          </b-dropdown-item-button>
        </b-dropdown-group>
        <b-dropdown-divider></b-dropdown-divider>
        <b-dropdown-item>
          <b-icon icon="power"></b-icon> logout
        </b-dropdown-item>
      </b-dropdown>
    </b-button-group>
  </b-button-toolbar>
</div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
.other {
  width: 50px;
}
</style>