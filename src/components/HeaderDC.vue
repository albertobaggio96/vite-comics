<script>
  export default {
    data(){
      return{
        navBarList: [
          {
            name : "characters",
            isActive : false
          },
          {
            name : "comics",
            isActive : true
          },
          {
            name : "movies",
            isActive : false
          },
          {
            name : "tv",
            isActive : false
          },
          {
            name : "games",
            isActive : false
          },
          {
            name : "collectibles",
            isActive : false
          },
          {
            name : "videos",
            isActive : false
          },
          {
            name : "fans",
            isActive : false
          },
          {
            name : "news",
            isActive : false
          },
          {
            name : "shop",
            isActive : false
          },
          
        ]
      }
    }
  }
</script>

<template>
  <header class="container">
    <nav class="d-flex align-items-center">
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <ul class="d-flex ms-auto mb-0">
        <li v-for="navBar in navBarList" :class=" navBar.isActive ? 'my-active' : ''" class="list-group-item me-3">{{ navBar.name.toUpperCase() }}</li>
      </ul>

    </nav>
  </header>
</template>

<style lang="scss" scoped>

img{
  width: 80px;
}

ul{
  font-weight: 600;
  li{
    line-height: 112px;
    font-size: small;
  }
}

</style>
