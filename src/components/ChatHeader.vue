<template>
  <div class="root d-flex align-items-center bg-light pr-3">
    <div class="d-flex align-items-center m-2 pl-1">
      <b-avatar variant="primary"></b-avatar>
      <div class="d-flex flex-column pl-1">
        <h4 class="m-0 p-0">Sharief</h4>
        <small>offline</small>
      </div>
    </div>
    <div style="margin-left: auto" class="d-flex align-items-center">
      <div class="searchbar">
        <div class="searchshape">
          <b-icon icon="search"></b-icon>
          <input type="search" class="input-search" placeholder="Search...">
        </div>
      </div>
      <div>
        <b-button-toolbar>
          <b-button-group>
            <b-dropdown variant="light" right no-caret>
              <template #button-content>
                <b-icon icon="paperclip"></b-icon>
              </template>
              <b-dropdown-item>
                <b-icon icon="link45deg"></b-icon> Link
              </b-dropdown-item>
              <b-dropdown-divider></b-dropdown-divider>
              <b-dropdown-group id="dropdown-group-1" header="Media">
                <b-dropdown-item>
                  <b-icon icon="image-fill"></b-icon> Image
                </b-dropdown-item>
                <b-dropdown-item-button>
                  <b-icon icon="file-earmark-richtext"></b-icon> Document
                </b-dropdown-item-button>
                <b-dropdown-item>
                  <b-icon icon="camera-video-fill"></b-icon> Video
                </b-dropdown-item>
              </b-dropdown-group>
            </b-dropdown>
            <b-dropdown variant="light" right no-caret>
              <template #button-content>
                <b-icon icon="three-dots-vertical"></b-icon>
              </template>
              <b-dropdown-item>
                <b-icon icon="person-fill"></b-icon> View Profile
              </b-dropdown-item>
              <b-dropdown-divider></b-dropdown-divider>
              <b-dropdown-group id="dropdown-group-1" header="Chat">
                <b-dropdown-item>
                  <b-icon icon="trash-fill"></b-icon> Clear Chat
                </b-dropdown-item>
                <b-dropdown-item-button>
                  <b-icon icon="reply-fill"></b-icon> Export Chat
                </b-dropdown-item-button>
              </b-dropdown-group>
              <b-dropdown-divider></b-dropdown-divider>
              <b-dropdown-item>
                <b-icon icon="person-x-fill"></b-icon> Block
              </b-dropdown-item>
            </b-dropdown>
          </b-button-group>
        </b-button-toolbar>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ChatHeader"
}
</script>

<style scoped>
.root {
  width: 100%;
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
</style>