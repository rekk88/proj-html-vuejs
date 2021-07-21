<template>
  <div class="main_wrap">
      <Jumbotron />
      <SiteDesc />
      <News />
      <BlogSection />
  </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import SiteDesc from './SiteDesc.vue'
import News from './News.vue'
import BlogSection from './BlogSection.vue'

export default {
    name:"Main",
    props:{
        //props in arrivo dal padre app
    },
    components:{
        Jumbotron,
        SiteDesc,
        News,
        BlogSection
    }
}
</script>

<style lang="scss" scoped>
    
</style>