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
$bg-c-main: #1c1c1c;
$text-white: #fff;
$d-flex:flex;
$f-direction-column:column;

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
  display: $d-flex;
  flex-direction: $f-direction-column;
  align-items: center;
  header{
    width: 80%;
    padding: 10px 0px;
  }
  main {
    text-align:left;
    background-color:$bg-c-main;
    color:$text-white;
    align-self: start;
    width: 100%;
    padding: 20px;



  }

}
</style>
