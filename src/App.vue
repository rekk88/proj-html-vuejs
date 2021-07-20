<template>
  <div id="app">
   
    <Header :menu="nav2"/>
    <Main /> <!-- sons : Jumbotron,-->
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
    Footer,
  },
  data() {
    return {
      nav2 : [
        {
          testo : "Home",
          visualizza : false
        },
        {
          testo : "Apple",
          visualizza : false
        },
        {
          testo : "Microsoft",
          visualizza : false
        },
        {
          testo : "Android",
          visualizza : false
        },
        {
          testo : "Forums",
          visualizza : false
        },
        {
          testo : "Contact us",
          visualizza : false
        }

      ]
    }
  },

}
</script>

<style lang="scss">
@import "./style/commons.scss"; 
@import url('https://fonts.googleapis.com/css2?family=Fira+Sans:wght@200;300;400;500;600;700&display=swap');
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-family: 'Fira Sans', sans-serif;
}
</style>
