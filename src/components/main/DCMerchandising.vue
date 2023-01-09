<script>
  export default {
    data(){
      return{
        merchandisingList:[
          {
            icon: "../../public/img/buy-comics-digital-comics.png",
            description: "Digital Comics"
          },
          {
            icon: "../../public/img/buy-comics-merchandise.png",
            description: "DC Merchandise"
          },
          {
            icon: "../../public/img/buy-comics-subscriptions.png",
            description: "Subscriptions"
          },
          {
            icon: "../../public/img/buy-comics-shop-locator.png",
            description: "Comic Shop Locator"
          },
          {
            icon: "../../public/img/buy-dc-power-visa.svg",
            description: "DC Power Visa"
          },
          
        ]
      }
    }
  }
</script>

<template>
  <section id="icon-banner" class="dc-bg-color">
    <div class="container py-5 d-flex justify-content-around">
        <div v-for="merchandising in merchandisingList" class="d-flex align-items-center">
          <img :src="`${merchandising.icon}`" :alt="merchandising.description" class="me-3">
          <div>{{ merchandising.description.toUpperCase() }}</div>
        </div>
    </div>
  </section>
</template>

<style lang="scss">
  img{
    width: 50px;
  }
</style>