<template>
  <div class="menu_wrap" @mouseenter="(visible = true)" @mouseleave="(visible = false)">

      <span>Forum</span>
      <div class="arrow-down" v-if="visible" @mouseenter="(visible = true)"></div>

      <div class="menu" v-if="visible"> <!-- v-if="visible"-->
          <ul class="px-3">
              <li class="py-3">item 1 Lorem, ipsum dolor.</li>
              <li class="py-3">item 2</li>
              <li class="py-3">item 3</li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    name:"Dropdown",
    data() {
        return {
            // listOne: false,
            visible : false
        }
    },
    props:{
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';

.menu{
    // visibility: hidden;
    position: absolute;
    color: black;
    // bottom: 100%;
    top: 80px;
    border: 1px solid black; //debug
    background-color: yellow; //debug
    ul{
        li{
            list-style: none;
            width: max-content;
            text-align: center;
            padding-left: 0;
            margin-left: 0;
            line-height: initial;
        }
    }
 
}
.test{
    display: block !important;
}

</style>