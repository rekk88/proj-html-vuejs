<template>
  <div class="container gallery_wrap">
      <!-- gallery first row -->
      <div class="row row-cols-4 gx-5 mb-4 text-center"> <!--mb-4 da modificare (troppo poco spazio)-->
          <div class="col">
              <ForumCard :icon="'fas fa-file-alt'" :text="'News & Community'"/>
          </div>
          <div class="col">
              <ForumCard :icon="'fab fa-apple'" :text="'Apple Forum'"/>
          </div>
          <div class="col">
              <ForumCard :icon="'fab fa-windows'" :text="'Windows Forum'"/>
          </div>
          <div class="col">
              <ForumCard :icon="'fab fa-android'" :text="'Android Forum'"/>
          </div>
      </div>
      <!-- end gallery first row -->
      <!-- gallery second row -->
     <div class="row row-cols-4 gx-5 text-center"> <!--mb-4 da modificare (troppo poco spazio)-->
          <div class="col">
              <ForumCard :icon="'fas fa-coffee'" :text="'General Discussion'"/>
          </div>
          <div class="col">
              <ForumCard :icon="'fas fa-boxes'" :text="'Apps & Software'"/>
          </div>
          <div class="col">
              <ForumCard :icon="'fas fa-laptop'" :text="'Gadgets & Stuff'"/>
          </div>
          <div class="col">
              <ForumCard :icon="'fas fa-wrench'" :text="'Apple Forum'"/>
          </div>
      </div>
      <!-- end gallery second row -->
      
      gallery test
  </div>
</template>

<script>
import ForumCard from './ForumCard.vue'

export default {
name:"ForumGallery",
components:{
    ForumCard
}


}
</script>

<style lang="scss" scoped>

</style>