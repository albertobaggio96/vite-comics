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
  <header>
    <HeaderDC/>
  </header>

  <main>
    <MainDC/>
  </main> 

  <footer>
    <FooterDC/>
  </footer>
</template>

<style>

</style>
