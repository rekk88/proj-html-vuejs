<template>
  <div class="main_wrap">
      <Jumbotron />
      <SiteDesc />
      <News />
  </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import SiteDesc from './SiteDesc.vue'
import News from './News.vue'


export default {
    name:"Main",
    props:{
        //props in arrivo dal padre app
    },
    components:{
        Jumbotron,
        SiteDesc,
        News
    }
}
</script>

<style lang="scss" scoped>
    
</style>