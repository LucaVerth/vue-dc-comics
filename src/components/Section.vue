<template>
  <section>
    <div class="central-banner">
      <div
        v-for="item in links" :key="item.id"
        class="shop-link"
      >
        <div class="shop-icon">
          <img :src="item.image" alt="">
        </div>
        <span class="shop-text">
          {{item.text}}
        </span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Section',
  data(){
    return {
      links: [
        {
          id: 1,
          image: require('../assets/img/buy-comics-digital-comics.png'),
          text: 'digital comics'
        },
        {
          id: 2,
          image: require('../assets/img/buy-comics-merchandise.png'),
          text: 'dc merchandise'
        },
        {
          id: 3,
          image: require('../assets/img/buy-comics-subscriptions.png'),
          text: 'subscription'
        },
        {
          id: 4,
          image: require('../assets/img/buy-comics-shop-locator.png'),
          text: 'comic shop locator'
        },
        {
          id: 5,
          image: require('../assets/img/buy-dc-power-visa.svg'),
          text: 'dc power visa'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import '../assets/style/mixins.scss';

section {
  background-color: #0282F9;
  .central-banner {
    @include container();
    @include align();
    justify-content: space-evenly;
    height: 150px;
  }
}
.shop-link {
  @include align();
  .shop-icon {
    width: 50px;
  }
  .shop-text{
    padding: 20px;
    text-transform: uppercase;
    font-size: 0.9rem;
  }
}
</style>