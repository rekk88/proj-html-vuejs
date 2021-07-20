<template>
  <div class="main_wrap">
      <Jumbotron />
      <SiteDesc />
  </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import SiteDesc from './SiteDesc.vue'

export default {
    name:"Main",
    props:{
        //props in arrivo dal padre app
    },
    components:{
        Jumbotron,
        SiteDesc
    }
}
</script>

<style lang="scss" scoped>
    
</style>