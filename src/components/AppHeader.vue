<script>
export default {
  name: "DC Header",
  data() {
    return {
      menuLinks: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
  methods: {
    toggleActive() {
      if ((this.menuLinks.current = true)) {
        this.menuLinks.current = false;
      } else {
        this.menuLinks.current = true;
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
        <li v-for="link in menuLinks">
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style scoped lang="scss">
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 1200px;
  margin: 0 auto;
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
        padding: 1.7rem 1rem;
        border-bottom: 5px solid transparent;
        &:hover {
          color: #0282f9;
          border-bottom: 5px solid #0282f9;
        }
      }
    }
  }
}
</style>
