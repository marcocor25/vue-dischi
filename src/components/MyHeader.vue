<template>
  <div class="header">
    <figure class="logo">
      <img src="../assets/img/logo.png" alt="Spotify" />
    </figure>
    <SearchBar />
  </div>
</template>

<script>
import SearchBar from "../components/SearchBar.vue";

export default {
  name: "MyHeader",
  components: {
    SearchBar,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header {
  min-height: 50px;
  padding: 0 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #2d3a46;

  .logo {
    width: 35px;
    height: 35px;
    border-radius: 50%;
    background: #000000;
  }
}
</style>
