<template>
  <div class="header_wrap ">
      <!-- Header -->
      <div class="container d-flex justify-content-around align-items-center">
            <div class="img_container">
                <img class="p-2" :src="require('@/assets/images/logo.png')" alt="logo">
            </div>
            <ul class="m-0 px-0">
                <li v-for="(element,index) in menu" :key="index" class="px-3">
                    {{element}}
                    <div class="arrow-down"></div>
                </li>
                <li class="ps-1"><span class="btn btn-dark px-4 text-uppercase">join us</span></li>
                <li><i class="fas fa-search ps-5 fs_6 align-middle"></i></li>
            </ul>
      </div>
      
  </div>
</template>

<script>
export default {
    name:"Header",
    props:{
        //props in arrivo dal padre app
        menu : Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
    .header_wrap{
        background-color: $eastern_blue;
        .container{
            height: 70px;
            .img_container{
                height: 100%;
                img{
                    height: 100%;
                }
            }
            ul{
                font-size: 0.95rem;
                color: $white;
                font-weight: bold;
                
                .btn.btn-dark{
                    font-weight: bold !important;
                    &:hover{
                        background-color: $salmon;
                        border-color: $salmon;
                    }
                }
            }

        }
    }
    li{
        list-style: none;
        display: inline-block;
    }
    // li:hover::after{
    //     display: inline-block;
    //     content: "";
    //     width: 0;
    //     height: 0;
    //     // border-left: 20px solid transparent;
    //     // border-right: 20px solid transparent;
    //     // border-top: 20px solid #f00;
    //     // border-width: 10px;
    //     border-style: solid;
    //     border-left: 10px;
    //     border-right: 10px;
    //     border-top: 8px;
    //     border-bottom: 8px;
    //     border-color: red;
    // }
    li:hover .arrow-down{
        display: block;
    }
</style>