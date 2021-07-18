<template>
  <div class="header_wrap ">
      <!-- Header -->
      <div class="container d-flex justify-content-between align-items-center">
            <div class="img_container">
                <img class="p-2" :src="require('@/assets/images/logo.png')" alt="logo">
            </div>
            <ul class="m-0 px-0">
                <!-- app -> prop menu -->
                <li v-for="(element,index) in menu" :key="index" class="px-3" @mouseenter="element.visualizza = true" @mouseleave="element.visualizza = false">
                    <span v-if="element.testo != 'Forums'">{{element.testo}}</span>
                    <span class="forum" v-else>
                        <Dropdown/>
                    </span>
                    <!-- v-if="(element.testo != 'Forums') così stampo a schermo la arrow-down all'interno di Dropdown -->
                    <div v-if="(element.testo != 'Forums') && (element.visualizza == true)" class="arrow-down"></div>
                </li>
                <ButtonBlue :color="'dark'" :textButton="'Join Us'"/>
                <li><i class="fas fa-search ps-5 fs_6 align-middle"></i></li>
            </ul>
           
      </div>
    
  </div>
</template>

<script>
import Dropdown from './Dropdown.vue'
import ButtonBlue from './ButtonBlue.vue'
export default {
    name:"Header",
    components: {
        Dropdown,
        ButtonBlue
    },
    props:{
        //props in arrivo dal padre app
        menu : Array
    },
    data() {
        return {
         
        }
    },
    methods:{
      

    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
    .header_wrap{
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
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
              
                // .btn.btn-dark{
                //     font-weight: bold !important;
                //     &:hover{
                //         background-color: $salmon;
                //         border-color: $salmon;
                //     }
                // }
            }

        }
    }
    li{
        list-style: none;
        display: inline-block;
        position:relative;
        line-height: 70px;
    }
    li:hover .arrow-down{
        display: block;

    }
</style>