<template>
  <select name="genre" id="select-genre">
    <option value="0" selected disabled>{{ selDefault }}</option>
    <option value="1">{{ selOne }}</option>
    <option value="2">{{ selTwo }}</option>
    <option value="3">{{ selThree }}</option>
    <option value="4">{{ selFour }}</option>
  </select>
</template>

<script>
export default {
  name: "SearchBar",
  data() {
    return {
      selDefault: "Generi",
      selOne: "Rock",
      selTwo: "Jazz",
      selThree: "Metal",
      selFour: "Pop",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#select-genre {
  min-width: 150px;
  min-height: 30px;
  padding: 0 5px;
  border: 0.5px solid #7b7e77;
  border-radius: 5px;
  font-size: 12px;
  font-weight: 700;
  text-transform: uppercase;
  color: #ffffff;
  background: #1c2d3b;

  &:focus-visible {
    outline: none;
  }
}
</style>
