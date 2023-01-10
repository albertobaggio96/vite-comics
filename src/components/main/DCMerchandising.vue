<script>
  export default {
    data(){
      return{
        merchandisingList:[
          {
            icon: "buy-comics-digital-comics.png",
            description: "Digital Comics"
          },
          {
            icon: "buy-comics-merchandise.png",
            description: "DC Merchandise"
          },
          {
            icon: "buy-comics-subscriptions.png",
            description: "Subscriptions"
          },
          {
            icon: "buy-comics-shop-locator.png",
            description: "Comic Shop Locator"
          },
          {
            icon: "buy-dc-power-visa.svg",
            description: "DC Power Visa"
          },
          
        ]
      }
    },
    methods: {
      getImagePath(imgPath){
        return new URL(`../../assets/img/${imgPath}`, import.meta.url).href;
      }
    },
  }
</script>

<template>
  <section id="icon-banner" class="dc-bg-color">
    <div class="container py-5 d-flex justify-content-around">
        <div v-for="merchandising in merchandisingList" class="d-flex align-items-center">
          <img :src="getImagePath(merchandising.icon)" :alt="merchandising.description" class="me-3">
          <div>{{ merchandising.description.toUpperCase() }}</div>
        </div>
    </div>
  </section>
</template>

<style lang="scss">
  #icon-banner{
    font-size: .9rem;
    
    img{
      width: 45px;
    }
  }

</style>