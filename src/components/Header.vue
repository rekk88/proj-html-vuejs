<template>
  <div class="header_wrap ">
      <!-- Header -->
      <div class="container d-flex justify-content-around align-items-center">
            <div class="img">
                <img :src="require('@/assets/images/logo.png')" alt="logo">
            </div>
            <ul class="m-0">
                <li v-for="(element,index) in menu" :key="index">{{element}}</li>
            </ul>
      </div>
      
  </div>
</template>

<script>
export default {
    name:"Header",
    props:{
        //props in arrivo dal padre app
        menu : Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
    .header_wrap{
        background-color: $eastern_blue;
    }
    li{
        list-style: none;
        display: inline-block;
    }


</style>