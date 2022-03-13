<template>
  <div class="main">
    <SearchBar />
    <div class="container">
      <MyCards
        v-for="(element, index) in cardsArray"
        :key="index"
        :cardsDetails="element"
      />
    </div>
  </div>
</template>

<script>
import SearchBar from "../components/SearchBar.vue";
import MyCards from "../components/MyCards.vue";
import axios from "axios";

export default {
  name: "MyMain",
  components: {
    SearchBar,
    MyCards,
  },
  data() {
    return {
      cardsArray: [],
    };
  },
  created() {
    axios
      .get("https://flynn.boolean.careers/exercises/api/array/music")
      .then((res) => {
        this.cardsArray = res.data.response;
      });
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  background: #1d2d3b;

  .container {
    width: 60vw;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
}
</style>
