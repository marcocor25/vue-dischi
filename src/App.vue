<template>
  <div id="app">
    <MyHeader />
    <MyMain />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyMain from "./components/MyMain.vue";

export default {
  name: "App",
  components: {
    MyHeader,
    MyMain,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/common.scss";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  width: 100%;
  height: 100%;
  display: block;
  user-select: none;
  -webkit-user-drag: none;
}

#app {
  height: 100vh;
  display: flex;
  flex-direction: column;
  font-family: Montserrat;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
}
</style>
