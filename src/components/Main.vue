<template>
  <div class="main_wrap">
      <Jumbotron />
  </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
export default {
    name:"Main",
    props:{
        //props in arrivo dal padre app
    },
    components:{
        Jumbotron
    }
}
</script>

<style lang="scss" scoped>
    
</style>