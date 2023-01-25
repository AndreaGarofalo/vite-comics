<script>
export default {
  name: "DC Header",
  props: {
    links: Array,
  },
  methods: {
    toggleActive() {
      if ((this.links.current = true)) {
        this.links.current = false;
      } else {
        this.links.current = true;
      }
    },
  },
};
</script>

<template>
  <header>
    <div class="container">
      <a href="#"><img src="../assets/img/dc-logo.png" alt="DC Logo" /></a>
      <ul>
        <li v-for="link in links" :key="link.text">
          <a :href="link.url" :class="{ active: link.current }">{{
            link.text
          }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style scoped lang="scss">
@use "../assets/scss/partials/mixins" as *;
@use "../assets/scss/partials/variables" as *;
header {
  background-color: $white;
}
.container {
  @include center("cross");
  justify-content: space-between;
  padding: 1rem;
  img {
    display: block;
    max-width: 3rem;
  }
  ul {
    display: flex;
    li {
      list-style-type: none;
      a {
        padding: 1.6rem 1rem;
        border-bottom: 5px solid transparent;
        &:hover {
          color: $blue;
          border-bottom: 4px solid $blue;
        }
        &.active {
          color: $blue;
          border-bottom: 4px solid $blue;
        }
      }
    }
  }
}
</style>
