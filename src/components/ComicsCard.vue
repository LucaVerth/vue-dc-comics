<template>
  <div class="card">
    <img :src="product.thumb" alt="">
    <h4>{{product.series}}</h4>
  </div>
</template>

<script>
export default {
  name: 'ComicsCard',
  props:{
    product: Object,
  }
}
</script>

<style lang="scss">
.card{
  width: calc((100% / 6) - 40px);
  margin: 10px 10px;
  padding-top: 40px;
}
</style>