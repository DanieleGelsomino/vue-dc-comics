<template>
  <div id="app">
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "variables";


*{
  padding:0px;
  margin:0px;
  box-sizing:border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
  }



}
</style>
