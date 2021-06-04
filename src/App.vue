<template>
  <div>
    <div class="main_tabs">
      <router-link class-active="active" to="/">Home</router-link>
      <router-link class-active="active" to="/About"
        >About me / Skills</router-link
      >
      <!-- <router-link class-active="active" to="/Skills">Skills</router-link> -->
      <router-link class-active="active" to="/Portfolio">Portfolio</router-link>
      <router-link class-active="active" to="/Contacts">Contacts</router-link>
    </div>
    <div class="container"></div>
    <div class="content">
      <router-view />
    </div>
  </div>
</template>

<style lang="scss">
@font-face {
  font-family: main-font-bold;
  src: url("assets/fonts/gilroy-bold.ttf");
}
@font-face {
  font-family: main-font-r;
  src: url("assets/fonts/gilroy-regular.ttf");
}
div {
  box-sizing: border-box;
}
body {
  font-family: sans-serif;
  font-family: "main-font-r" !important;
}
.container {
  position: relative;
}
.content {
  height: 95vh;
  position: relative;
}
.main_tabs {
  display: grid;
  width: 100%;
  grid-template-columns: repeat(5, 1fr);
  background-color: #ccc;
  height: 5vh;
  align-items: center;
  a {
    font-size: 18px;
    text-align: center;
    font-weight: bold;
    font-family: "main-font-r";
    color: #828282;
    text-transform: uppercase;
    text-decoration: none;
    &.router-link-active.router-link-exact-active {
      color: #070707;
      border-bottom: 2px solid #000;
    }
  }
}
</style>
