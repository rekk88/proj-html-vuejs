<template>
  <div class="hero_wrap mx-1">
      <div class="text_wrap">
        <div>riga 1 testo</div>
        <h3>riga 1 testo</h3>
        <div>riga 1 testo</div>
        <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum sadips ets ipsums dolores ficilis uns leo lectus.</p>
        <div class="btn btn-dark">Button test</div>
      </div>
      
  </div>
</template>

<script>
export default {
name: "Hero"
}
</script>

<style lang="scss" scoped>  
.hero_wrap{
    background-image: url("../assets/images/featured_article_1_bg.jpg"); //to enter as prop
    background-size: cover;
    height: 600px;
    position: relative;
    .text_wrap{
        position: absolute;
        bottom: 100px;
        padding: 0px 50px;
    }
}
</style>