<template>
  <div class="community_wrap text-center">
      <div class="w-50">
        <h2 class="fs-1">Hey! Join our Community</h2>
        <p>Nulla molestie tortor nec lectus venenatis, 
            sed blandit dui finibus. Curabitur feugiat vulputate purus ipsums dolores ficilis uns etra.
        </p>
        <Button :color="'blue'" :textButton="'Sign up >'" :paddinTopBottom="'0.7rem'" :paddingLeftRight="'2.5rem'"/>

      </div>
      
  </div>
</template>

<script>
import Button from './Button.vue'


export default {
name:"Community",
components:{
    Button
}

}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
.community_wrap{
    background-image: url('../assets/images/join_now_cta_bg.jpg');
    background-size: cover;
    color: $white;
    div{
        margin: 0 auto;
        padding: 10rem 0rem;
    }
}
</style>