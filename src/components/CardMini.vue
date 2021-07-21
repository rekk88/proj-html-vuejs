<template>
  <div class="my-2">
      <img :src="require('../assets/images/' + imgPath)" alt="img test">
      <div class="text">
          <h6 class="fs-5">{{titolo}}</h6>
           <div class="date_comments">
              <span>{{date}}</span><span> | </span> <span class="comments" v-if="comments > 0">{{comments}} comments</span> <span class="comments_off" v-else> Comments off</span>
          </div>
      </div>
  </div>
</template>

<script>
export default {
name:"CardMini",
props:{
    imgPath : String,
    date : String,
    titolo: String,
    comments : Number
}
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
img{
    width: 40%;
    vertical-align: top;
}
.text{
    margin-left: 15px;
    width: calc(60% - 15px);
    display: inline-block;
}
.date_comments{
        font-size: 0.80rem;
        & :nth-child(1),:nth-child(2){ //nth-child di .comments
            color: $nevada;
        }
        .comments{
            color: $cape_code;
        }
        .comments_off{
            color: $nevada;
        }

    }
</style>