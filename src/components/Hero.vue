<template>
<!-- <div class="circular" v-bind:style="{ backgroundImage: 'url(' + image + ')' }" -->
  <div class="hero_wrap" :style="'backgroundImage: '+'url(' + background + ')' ">
      <div class="text_wrap">
        <h6>{{titleH6}}</h6>
        <h2 class="fs-1 fw-bold py-3">{{titleH2}}</h2>
        <p class="fs-6">In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum sadips ets ipsums dolores ficilis uns leo lectus.</p>
        <!-- <div class="btn btn-dark">Button test</div> -->
        <Button :color="'dark'" :textButton="'read more >'" :paddinTopBottom="'0.8rem'" :paddingLeftRight="'2.5rem'"/>
      </div>
      
  </div>
</template>

<script>
import Button from './Button.vue'


export default {
name: "Hero",
components:{
  Button
},
props:{
  titleH6 : String,
  titleH2 : String,
  background : Text
}
}
</script>

<style lang="scss" scoped>  
.hero_wrap{
    // background-image: url("../assets/images/featured_article_1_bg.jpg"); //to enter as prop
    background-size: cover;
    color: white;
    .text_wrap{
        padding: 0px 50px;
        padding-top: 20%;
        padding-bottom: 10%;
        h6{
          text-transform: uppercase;
          letter-spacing: 5px;
        }
        p{
          font-weight: 500;
        }
    }
}
</style>