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
.card-list {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
}
.card{
    flex-basis: calc(100% /6);
    margin: 40px 0;
    padding: 0 20px;
}

</style>