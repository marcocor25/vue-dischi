<template>
  <div class="main">
    <div class="container">
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
      <div class="card">
        <figure class="card-image"></figure>
        <h3>title</h3>
        <p>mario rossi</p>
        <p>2022</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyMain",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main {
  flex-grow: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #1d2d3b;

  .container {
    width: 60vw;
    min-height: 10vh;
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    border: 2px dashed yellow;

    .card {
      flex-grow: 1;
      padding: 10px;
      width: calc((100% / 5) - 20px);
      height: 220px;
      text-align: center;
      background: #2d3a46;

      .card-image {
        aspect-ratio: 1/1;
        background: rebeccapurple;
      }

      h3 {
        padding: 10px 0;
        text-transform: uppercase;
      }

      p {
        text-transform: capitalize;
        font-size: 12px;
        color: #7b7e77;
      }
    }
  }
}
</style>
