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
  <footer class="text-white">
    
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
            <img src="../../public/img/dc-logo-bg.png" alt="dc logo" class="w-100">
          </figure>
        </div>
      </section>
  
      <section id="footer-bottom" class="container d-flex py-4 align-items-center">
        <button class="text-white border-2 p-2 fs-5">SIGN-UP NOW!</button>
        <div class="ms-auto fs-5">FOLLOW US</div>
        <img src="../../public/img/footer-facebook.png" alt="Facebook" class="ps-3">
        <img src="../../public/img/footer-twitter.png" alt="Twitter" class="ps-3">
        <img src="../../public/img/footer-youtube.png" alt="Twitter" class="ps-3">
        <img src="../../public/img/footer-pinterest.png" alt="Pinterest" class="ps-3">
        <img src="../../public/img/footer-periscope.png" alt="Periscope" class="ps-3">
      </section>
    </footer>
</template>

<style lang="scss" scoped>
  @use "../styles/partials/variables" as *;


  footer{
    background-color: $footer-color;

    #footer-links{
      background-image: url("../../public/img/footer-bg.jpg");
      background-repeat: no-repeat;
      background-size: cover;
      .container{
        height: 330px;     
      
        div{
          width: 165px;
      
          li{
            font-size: small;
  
          }
        }
      }
  
      
    }
  
    #footer-bottom{
      button {
        border-color: $DC-color;
        background-color: $footer-color;
      }
      div{
        font-weight: bolder;
        color: $DC-color
      }
    }
  }
  
</style>