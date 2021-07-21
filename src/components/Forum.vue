<template>
<div class="forum_wrap">
    <SectionTitle :titoloh6="'PHASELLUS EGET METUS'" :titoloH2="'Forum Sections'"/>
    <ForumGallery />
</div>
</template>

<script>
import SectionTitle from './SectionTitle.vue'
import ForumGallery from './ForumGallery.vue'

export default {
name:"Forum",
components:{
    SectionTitle,
    ForumGallery

}
}
</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';
.forum_wrap{
    background-color: $light_grey;
}
</style>