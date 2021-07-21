<template>
  <div class="secTitle_wrap">
      <div class="container text-center">
        <h6>{{titoloh6}}</h6>
        <h2 class="fw-bold fs-1 mb-5">{{titoloH2}}</h2>
        <div>
            <div class="underline"></div>
        </div>
      </div>
     
  </div>
</template>

<script>
export default {
name:"SectionTitle",
data(){
    return{

    }
},
props:{
    titoloh6: String,
    titoloH2: String
}
}

</script>

<style lang="scss" scoped>
@import '@/style/colors.scss';

.secTitle_wrap{
    margin-top: 6rem;
    margin-bottom: 6rem;
    h6{
        letter-spacing: 5px;
        color: $cape_code;
    }
    .underline{
        border-top: 2px solid;
        border-color: orange;
        width: 8%;
        max-width: 102px;
        margin: 0 auto;
    }
}
</style>