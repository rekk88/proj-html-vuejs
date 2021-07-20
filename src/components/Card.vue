<template>
  <div>
      <img :src="require('../assets/images/' + imgPath)" alt="img test">
      <div class="card_text">
          <h5 class="fw-bold mt-2 mb-0">Morbi vitae dui euismod vulputate sollicitudin</h5>
          <div class="date_comments">
              <span>{{date}}</span><span> | </span> <span class="comments" v-if="comments > 0">{{comments}} comments</span> <span class="comments_off" v-else> Comments off</span>
          </div>
          <p class="img_desc mt-3">Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl</p>
          <!--  <span>October 11th, 2015</span><span> | </span> <span>2 comments</span>-->
      </div>
  </div>
</template>

<script>
export default {
name:"Card",
props:{
    imgPath : String,
    date : String, //post date
    comments : Number // number of comments
}
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';

img{
    width: 100%;
}
.card_text{
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
    .img_desc{
        color: $nevada;
    }
}
</style>