<template>
  <div class="card_wrap pb_6">
      <!-- <i class="fontawesome-icon forum-file-text circle-yes"> -->
          <div class="rounded-circle mt-5 mb-3">
            <i :class="icon+' fs-2' "></i>
          </div>
          <div class="w-100 fw-bold">
             {{text}}
          </div>
  </div>
</template>

<script>
export default {
name:"ForumCard",
props:{
    icon : String,
    text : String
}
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
.card_wrap{
    width: 90%;
    margin: 0 auto;
    background-color: $white;
    border-top: 2px solid $eastern_blue;
    div.rounded-circle{
        display: inline-block;
        padding: 15px 20px;
        background-color: $salmon;
        i{
            color: $white;
            background-color: $salmon;
        }
    }
  
}
</style>