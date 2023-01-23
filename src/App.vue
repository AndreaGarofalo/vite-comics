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
  <div class="body">
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.body {
  width: 100vw;
  height: 100vh;
}
</style>
