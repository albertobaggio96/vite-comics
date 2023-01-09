<script>
  export default {
    data(){
      return{
        footerLists :[
          {
            title: "dc comics",
            list : ["Characters", "Comics", "Movies", "Tv", "Games", "Collectibles", "Videos", "Fans", "News", "Shop",]
          },
          {
            title: "shop",
            list : ["Shop DC", "Shop DC Collectibles"]
          },
          {
            title: "dc",
            list : ["Terme Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscritions", "Talent Workshops","CPSC Certificates", "Ratings", "Shop Help", "Contact Us"]
          },
          {
            title: "sites",
            list : ["DC", "MAD Magazine", "DC kids", "DC Universe", "DC Power Visa"]
          },
        ]

      }
    }
  }
</script>

<template>
  <footer class="bg-dark text-white">
    
    <section id="footer-links" class="py-5 overflow-hidden">
        <div class="container position-relative">
          <div class=" d-flex flex-column flex-wrap h-100">
            <article v-for="footerUl in footerLists" class="w-100">
              <h2 class="fs-5 ">{{ footerUl.title.toUpperCase()}}</h2>
              <ul class="ps-0">
                <li v-for="footerLink in footerUl.list" class="list-group-item text-secondary">{{ footerLink }}</li>
              </ul>
            </article>
          </div>
          <figure class="position-absolute top-50 end-0 translate-middle-y">
            <img src="../assets/img/dc-logo-bg.png" alt="" >
          </figure>
        </div>
      </section>
  
      <section id="footer-bottom" class="container bg-dark d-flex">
        <button>SIGN-UP NOW!</button>
        <div class="ms-auto">social</div>
      </section>
    </footer>
</template>

<style lang="scss" scoped>

#footer-links{
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  .container{
    height: 330px; 
    
    // display: flex;
    // flex-direction: column;
    // flex-wrap: wrap;
    
  
    div{

      width: 165px;
  
      li{
        font-size: small;
      }
    }
  }
  
}
  
</style>