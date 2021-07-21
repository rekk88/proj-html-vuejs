<template>
  <div class="jumbo_wrap">
      <div class="text container d-flex align-items-center">
          <div>
            <h1 class="my-0">Tech Forum!</h1>
            <p class="pb-5 my-0">Discuss all the latest technology news and trends</p>
            <!-- <div class="btn btn-dark">Button</div> -->
            <Button :color="'blue'" :textButton="'Get avada now! >'" :paddinTopBottom="'0.7rem'" :paddingLeftRight="'2.5rem'"/>
          </div>
      </div>
  </div>
</template>

<script>
import Button from './Button.vue'

export default {
    name:"Jumbotron",
    components:{
        Button
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
.jumbo_wrap{
    background-image: url("../assets/images/home_slider_bg.jpg");
    height: 100vh;
    background-attachment: fixed;
    margin-top: 70px;
    color: $white;
    .text.container{
        height: 100%;
        h1{
            font-size: 7rem;
        }
        p{
            font-size: 2rem;
        }
    }
}
</style>