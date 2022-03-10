<template>
  <div class="card">
    <figure class="card-image">
      <img :src="cardsDetails.poster" :alt="cardsDetails.title" />
    </figure>
    <h5>{{ cardsDetails.title }}</h5>
    <p>{{ cardsDetails.author }}</p>
    <p>{{ cardsDetails.year }}</p>
  </div>
</template>

<script>
export default {
  name: "MyCards",
  props: {
    cardsDetails: {
      type: Object,
      required: true,
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card {
  flex-grow: 1;
  width: calc((100% / 5) - 20px);
  min-height: 240px;
  padding: 12px;
  text-align: center;
  cursor: pointer;
  background: #2d3a46;

  .card-image {
    aspect-ratio: 1/1;
  }

  h5 {
    padding: 10px 0;
    text-transform: uppercase;
  }

  p {
    text-transform: capitalize;
    font-size: 12px;
    color: #7b7e77;
  }
}
</style>
