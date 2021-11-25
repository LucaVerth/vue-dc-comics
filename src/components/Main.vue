<template>
  <main>
    <Jumbotron/>
    <div class="main-container">
      <div class="card-list">
        <Comics
          v-for="(product, index) in ProductsItems"
          :key="index"
          :product="product"
        />
      </div>
      
    </div>
  </main>
</template>

<script>
import Comics from './ComicsCard.vue';
import Jumbotron from './Jumbotron.vue';
import ProductsItems from '../assets/data/products.js';

export default {
  name: 'Main',
  components:{
    Comics,
    Jumbotron,
  },
  data(){
    return {
      ProductsItems,
    }
  }
}
</script>

<style lang="scss">
@import '../assets/style/mixins.scss';

main{
  background-color: #000;
  color: #fff;
  .main-container{
    @include container();
    @include align();
    min-height: 100px;
  }
}
</style>