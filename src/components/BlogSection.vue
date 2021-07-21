<template>
       <div class="blog">
      <div class="blog_text text-center fw-bold fs-5 text-uppercase">
          read our blog ->
      </div>
  </div>
 
</template>

<script>
export default {
name:"BlogSection"
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