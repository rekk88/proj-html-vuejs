<template>
  <div class="main_wrap">
      <Jumbotron />
      <SiteDesc />
      <News />
      <BlogSection />
      <Forum />
  </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import SiteDesc from './SiteDesc.vue'
import News from './News.vue'
import BlogSection from './BlogSection.vue'
import Forum from './Forum.vue'

export default {
    name:"Main",
    props:{
        //props in arrivo dal padre app
    },
    components:{
        Jumbotron,
        SiteDesc,
        News,
        BlogSection,
        Forum
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors';

.main_wrap{
    background-color: $light_grey;
}
</style>