<template>
  <div class="siteDesc_wrap  text-center">
       <div class="container py_7">
          <h6 class="descTitle"> AVADA FORUM IS THE PLACE TO BE</h6>
          <p class="fs-4 descP">
            In quis lectus sed leo elementum faucibus in dapibus dictum. 
            Nulla molestie tortor nec lectus venenatis, sed blandit dui 
            finibus. dolor at, bibendum purus. 
            Donec vehicula nec tortor ac finibus.
          </p>
       </div>
  </div>
</template>

<script>
export default {
    name:"SiteDesc"
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
.siteDesc_wrap{
  background-color: $light_grey;
  .container{
      .descTitle{
        word-spacing: 10px;
        color: $cape_code;
      }
      .descP{
        margin: 0 auto;
        width: 70%;
        color:$nevada;
      }
  }
}
</style>