<script>
export default {
  name: "DC Merchandise",
};
</script>

<template>
  <section class="merchandise">
    <div class="container">
      <a href="#">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
        <h2>DIGITAL COMICS</h2>
      </a>
      <a href="#">
        <img src="../assets/img/buy-comics-merchandise.png" alt="" />
        <h2>DC MERCHANDISE</h2>
      </a>
      <a href="#">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
        <h2>SUBSCRIPTIONS</h2>
      </a>
      <a href="#">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
        <h2>COMIC SHOP LOCATOR</h2>
      </a>
      <a href="#">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
        <h2>DC POWER VISA</h2>
      </a>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use "../assets/scss/partials/mixins" as *;
@use "../assets/scss/partials/variables" as *;
.merchandise {
  height: 10rem;
  background-color: $blue;
  .container {
    height: 100%;
    @include center("both");
    justify-content: space-around;
    a {
      display: flex;
      @include center("both");
      h2 {
        color: white;
        font-size: 18px;
      }
      img {
        height: 50px;
      }
    }
  }
}
</style>
