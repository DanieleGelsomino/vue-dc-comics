<template>
  <div id="app">
    <Header :links="menu" />
    <Main :comicsSeries="comics" />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import headerMenu from "@/data/menu";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      menu: headerMenu,
    };
  },
};
</script>

<style lang="scss">
@import "variables";

* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
}

#app {
  font-family: "DM Sans", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: $d-flex;
  flex-direction: $f-direction-column;
  justify-content: center;
  background-color: #000;
  height: 100vh;
  header {
    background-color: #fff;
    display: $d-flex;
    justify-content: center;
    padding: 10px 0px;
  }
  main {
    background-color: $bg-c-main;
    display: $d-flex;
    justify-content: center;
    padding: 30px 0px;
    flex-grow: 1;
  }
}
</style>
