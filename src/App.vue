<script>
import HeaderDC from './components/HeaderDC.vue'
import MainDC from './components/MainDC.vue'
import FooterDC from './components/FooterVue.vue'

export default{
  components : {
    HeaderDC,
    MainDC,
    FooterDC
  }
}
</script>

<template>
    <HeaderDC/>

    <MainDC/>

    <FooterDC/>
</template>

<style lang="scss">
  @use "./styles/partials/variables" as *;
  @use "./styles/general.scss" as *;
  @use "../node_modules/bootstrap/scss/bootstrap.scss" as *;

  #content{
    background-color: $content-color;
  }

  .dc-bg-color{
    background-color: $DC-color;
  }
  .my-active{
    color: $DC-color;
    border-bottom: 5px solid $DC-color;
  }
</style>
