<template>
       <div class="blog">
      <div class="blog_text text-center fw-bold fs-5 text-uppercase">
          {{text}}
      </div>
  </div>
 
</template>

<script>
export default {
name:"BlackSpacer",
props:{
    text : String
}
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
.blog{
 background-color: black;
 color: $white;
 .blog_text{
     padding: 60px 0px;
 }
}

</style>