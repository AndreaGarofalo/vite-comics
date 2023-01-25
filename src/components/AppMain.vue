<script>
export default {
  name: "DC Content",
  props: {
    products: Array,
  },
};
</script>

<template>
  <main>
    <div class="container">
      <div class="cards-row">
        <div v-for="product in products" :key="product.thumb" class="card-col">
          <figure>
            <img :src="product.thumb" :alt="product.series" />
          </figure>
          <figcaption>{{ product.series }}</figcaption>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped lang="scss">
@use "../assets/scss/partials/mixins" as *;
@use "../assets/scss/partials/variables" as *;
main {
  background-color: $black;
  .container {
    .cards-row {
      display: flex;
      flex-wrap: wrap;
      padding-bottom: 2rem;
      .card-col {
        flex-basis: calc(100% / 6);
        margin-top: 2rem;

        overflow: hidden;
        figure {
          height: 200px;
          width: 200px;
          padding: 10px;
          overflow: hidden;
        }
        figcaption {
          padding: 10px;
          color: $white;
          font-size: 16px;
        }
      }
    }
  }
}
</style>
