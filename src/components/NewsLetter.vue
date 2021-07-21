<template>
  <div class="newsLetter_wrap text-center py-5">
      <h3>Subscribe to our newsletter</h3>
      <div>
          <input class="me-2" type="text" placeholder="Email : ">
          <Button :color="'black'" :textButton="'Sign up >'" :paddinTopBottom="'0.4rem'" :paddingLeftRight="'2.5rem'"/>
          
      </div>
  </div>
</template>

<script>
import Button from './Button.vue'
export default {
name:"NewsLetter",
components:{
    Button
}
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';

.newsLetter_wrap{
    background-color: $light_grey;
    input{
        height: 40px;
        border: none;
        max-width: 400px;
        width: 100%;
    }
}
</style>