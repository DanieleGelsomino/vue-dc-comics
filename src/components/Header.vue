<template>
  <header>
    <div class="dc-navbar">
      <!-- logo dc piccolo -->
      <img class="logo-small" src="../assets/dc-logo.png" alt="dc-logo-small" />
      <!-- navbar menu -->
      <ul>
        <li
          v-for="(item, index) in links"
          :key="index"
          :class="{ active: item.active }"
        >
          <a href="#">{{ item.name }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  props: {
    links: Array,
  },
};
</script>

<style scope lang="scss">
@import "@/variables";

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
      &.active {
        color: $text-azure;
        border-bottom: 5px solid $text-azure;
      }
      a {
        text-decoration: $no-decoration;
        color: $text-darkgray;
        padding-bottom: 30px;
      }
    }
  }
}
</style>