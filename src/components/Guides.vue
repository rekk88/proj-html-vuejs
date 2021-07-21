<template>
  <div class="guides_wrap">
      <div class="container">
        <!-- title guide -->
        <div class="title_guide">
            <h2 class="fw-bold mb-3">{{titoloH2}}</h2>
            <div>
                <div class="underline mb-3"></div>
            </div>
        </div>
        
        <!-- end title guide -->
        <div class="testc">
            <CardMini :imgPath="'post_feat_img_20-177x142.jpg'" :date="'October 11th, 2015'" :comments="0" :titolo="'Donec ornare pretium eget scelisque justo'"/>
            <CardMini :imgPath="'post_feat_img_22-177x142.jpg'" :date="'October 11th, 2015'" :comments="0" :titolo="'Donec ornare pretium eget scelisque justo'"/>
            <CardMini :imgPath="'post_feat_img_23-177x142.jpg'" :date="'October 11th, 2015'" :comments="0" :titolo="'Donec ornare pretium eget scelisque justo'"/>
        </div>

      </div>
  </div>
</template>

<script>
import CardMini from './CardMini.vue'
export default {
name:"Guides",
components:{
    CardMini
},
props:{
    titoloH2: String
},
}
</script>

<style lang="scss" scoped>
.container{
    height: 80%;
}
.title_guide{
    height: 20%;
}

.guides_wrap{
    height: 100%;
}
.underline{
        border-top: 2px solid;
        border-color: orange;
        width: 25%;
        max-width: 102px;
}
.testc{
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
</style>