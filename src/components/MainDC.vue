<script>
  import JumboMain from "./main/JumboMain.vue";
  import CurrentSeriesMain from "./main/CurrentSeriesMain.vue";
  import DCMerchandising from "./main/DCMerchandising.vue"
  export default {
    components: {
      JumboMain,
      CurrentSeriesMain,
      DCMerchandising,
    }
  }
</script>

<template>
  <main class="text-white">
    <JumboMain/>

    <CurrentSeriesMain/>

    <DCMerchandising/>

  </main>
</template>
  
<style lang="scss">

</style>