<template>
    <ul class="ps-0">
    <li class="">
        <span :class="'btn btn-'+color+ ' text-uppercase'" :style="'padding: ' + paddinTopBottom + ' ' + paddingLeftRight">{{textButton}}</span>
    </li>
    </ul>
</template>

<script>
export default {
    name:"Button",
    props:{
        color: String,
        textButton: String,
        paddinTopBottom:String,
        paddingLeftRight:String
    },
    data(){
        return{
            // top: paddinTopBottom,
            // bottom: paddinTopBottom,

        }
    },
    // computed:{
    //     cssProps(){
    //         return 'padding: ' + this.top + ' ' + 0
    //     }
    // }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
ul{
    display: inline-block;
    li{
        list-style: none;
        padding-top: var(--top);
        padding-bottom: var(--bottom);

    }
}

.btn{
    color: $white !important;
    font-weight: bold !important;
        &:hover{
            background-color: $salmon;
            border-color: $salmon;
        }
}


</style>