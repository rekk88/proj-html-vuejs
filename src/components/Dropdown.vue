<template>
  <div class="menu_wrap" @mouseenter="(visible = true)" @mouseleave="(visible = false)">

      <span>Forum</span>
      <div class="arrow-down" v-if="visible" @mouseenter="(visible = true)"></div>
      <div class="arrow-up" v-if="visible" @mouseenter="(visible = true)"></div>

      <div class="menu" v-if="visible"> <!-- v-if="visible"-->
          <ul class="px-3">
              <li v-for="(item,index) in items" :key="index" class="py-3">{{item}}</li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    name:"Dropdown",
    data() {
        return {
            visible : false,
            items : ["Apple","Android","Microsoft","Apps & Software","Gadgets & Stuff","General Discussion","News & Community","Tutorials & Guide"]
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
    top: 94px;
    border: 1px solid black; //debug
    background-color: $white; //debug
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
.arrow-up{
    top: 84px;
    border-bottom-color: $white;
}
.test{
    display: block !important;
}

</style>