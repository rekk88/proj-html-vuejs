<template>
  <div id="app">
   
    <Header :menu="nav"/>
    <Main />
    <Footer />
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
  },
  data() {
    return {
      nav : ["Home","Apple","Microsoft","Android","Forums","Contact us"],
    }
  },

}
</script>

<style lang="scss">
@import "./style/commons.scss"; 

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
