<template>
  <div class="main_wrap">
      <Jumbotron />
      <SiteDesc />
      <News />
      <BlackSpacer :text="'read our blog ->'"/>
      <Forum />
      <BlackSpacer :text="'go to our forum ->'"/>
      <Community />
      <NewsLetter />
  </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import SiteDesc from './SiteDesc.vue'
import News from './News.vue'
import BlackSpacer from './BlackSpacer.vue'
import Forum from './Forum.vue'
import Community from './Community.vue'
import NewsLetter from './NewsLetter.vue'

export default {
    name:"Main",
    props:{
        //props in arrivo dal padre app
    },
    components:{
        Jumbotron,
        SiteDesc,
        News,
        BlackSpacer,
        Forum,
        Community,
        NewsLetter
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors';

.main_wrap{
    background-color: $white;
}
</style>