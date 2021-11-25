<template>
  <main>
    <Jumbotron/>
    <div class="main-container">
      <div class="card-list">
        <div class="custom-btn-main">Current Series</div>
        <Comics
          v-for="(product, index) in ProductsItems"
          :key="index"
          :product="product"
        />
      </div>
    </div>
    <div class="load-btn">
      <div class="custom-btn"><a href="#">load more</a></div>
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
    position: relative;
    @include container();
    @include align();
    min-height: 100px;
  }
  .load-btn{
    display: flex;
    justify-content: center;
    padding: 20px;
    .custom-btn{
      @include button();
      width: 250px;
      height: 40px;
      background-color: #0282F9;
    }
  }
  .custom-btn-main{
    position: absolute;
    top: -20px;
    left: 50px;
    @include button();
    width: 200px;
    height: 40px;
    background-color: #0282F9;
    font-weight: bold;
    font-size: 1.2rem;
  }
  
}
.card-list {
  width: 100%;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
</style>