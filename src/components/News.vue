<template>
  <div class="container">
      <SectionTitle :titoloh6="'PHASELLUS EGET METUS'" :titoloH2="'All the latest news'"/>
      <!-- card top row -->
      <div class="row row-cols-3 my-2">
          <Card :imgPath="'post_feat_img_25-700x441.jpg'" :date="'October 11th, 2015'" :comments="2"/>
          <Card :imgPath="'post_feat_img_24-700x441.jpg'" :date="'October 11th, 2015'" :comments="0"/>
          <Card :imgPath="'post_feat_img_23-700x441.jpg'" :date="'October 11th, 2015'" :comments="0"/>
      </div>
      <!-- end card top row -->
      <!-- central row -->
      <div class="row row-cols-1 mx-1">
          <!-- test central row -->
          <Hero />
      </div>
      <!-- end central row -->
      <!-- card bottom row -->
      <div class="row row-cols-3 my-2 px-0">
          <Card :imgPath="'post_feat_img_25-700x441.jpg'" :date="'October 11th, 2015'" :comments="2"/>
          <Card :imgPath="'post_feat_img_24-700x441.jpg'" :date="'October 11th, 2015'" :comments="0"/>
          <Card :imgPath="'post_feat_img_23-700x441.jpg'" :date="'October 11th, 2015'" :comments="0"/>
      </div>
      <!-- end card bottom row -->
  </div>
</template>

<script>
import SectionTitle from './SectionTitle.vue'
import Card from './Card.vue'
import Hero from './Hero.vue'

export default {
name:"News",
props:{

},
components:{
    SectionTitle,
    Card,
    Hero
}

}
</script>

<style lang="scss" scoped>

</style>