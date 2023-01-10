<script>
export default {
  props : [
    "thumb",
    "price",
    "series",
    "type"
  ]
}
</script>

<template>
    <article>
      <figure class="text-center">
        <img :src="thumb" :alt="series" >
      </figure>
      <h3 class="pb-5">{{ series.toUpperCase() }}</h3>
    </article>
</template>

<style lang="scss">
  article{
    width: calc(100% / 6);
    width: 150px;
    

    img{
      width: 100%;
      height: 150px;
      object-fit: cover;
      object-position: top;
    }
    h3{
      font-size: small;
    }
  } 
</style>