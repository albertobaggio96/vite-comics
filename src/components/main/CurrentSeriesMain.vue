<script>
export default {
  props : [
    "thumb",
    "price",
    "series"
  ]
}
</script>

<template>
    <article >
      <div class="text-center position-relative mb-3">
        <img :src="thumb" :alt="series" >
        <div class="position-absolute bg-dark bg-opacity-75">{{ price }}</div>
      </div>
      <h3 class="pb-4">{{ series.toUpperCase() }}</h3>
    </article>
</template>

<style lang="scss">
  article{
    width: calc(100% / 6);
    width: 150px;

    div.position-relative{
      height: 150px;

      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
      }

      div{
        right: 0;
        bottom: 0;
        display: none;
      }

      &:hover div{
        display: block;
      }
    }

    h3{
      font-size: small;
    }
  } 
</style>