<template>
    <li class="ps-1"><span :class="'btn btn-'+color+ ' px-4 text-uppercase'">{{textButton}}</span></li>
</template>

<script>
export default {
    name:"ButtonBlue",
    props:{
        color: String,
        textButton: String
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
li{
    list-style: none;
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