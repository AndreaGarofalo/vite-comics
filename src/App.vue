<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  data() {
    return {};
  },
  components: { AppHeader, AppMain, AppFooter },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: "Open Sans";
  min-height: 100vh;
  background-image: url("./assets/img/footer-bg.jpg");
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
}
img {
  max-width: 100%;
  height: auto;
}
a {
  color: black;
  text-decoration: none;
}

/* Utility */

.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
