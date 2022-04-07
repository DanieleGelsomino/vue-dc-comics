<template>
  <header>
    <div class="dc-navbar">
      <!-- logo dc piccolo -->
      <img class="logo-small" src="../assets/dc-logo.png" alt="dc-logo-small" />
      <!-- navbar menu -->
      <ul>
        <li v-for="item in menu" :key="item.name">
          <a href="#"></a>{{ item.name }}
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      menu: [
        {
          name: "characters",
          active: false,
        },
        {
          name: "comics",
          active: false,
        },
        {
          name: "movies",
          active: false,
        },
        {
          name: "tv",
          active: false,
        },
        {
          name: "games",
          active: false,
        },
        {
          name: "collectibles",
          active: false,
        },
        {
          name: "videos",
          active: false,
        },
        {
          name: "fans",
          active: false,
        },
        {
          name: "news",
          active: false,
        },
        {
          name: "shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scope lang="scss">
@import "../variables";

.dc-navbar {
  display: $d-flex;
  justify-content: space-between;
  align-items: center;
  width: $w-80;
  .logo-small {
    width: 60px;
    height: 60px;
  }
  ul {
    display: $d-flex;
    list-style-type: $list-style;
    flex-wrap: wrap;
    li {
      font-size: $font-size-6;
      font-weight: $text-bold;
      text-transform: $text-uppercase;
      margin: 0 10px;
      a {
        text-decoration: $no-decoration;
        color: $text-darkgray;
        padding-bottom: 30px;
        &:hover {
          color: $text-azure;
          border-bottom: 5px solid $text-azure;
        }
      }
    }
  }
}
</style>