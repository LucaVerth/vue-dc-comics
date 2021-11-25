<template>
  <main>
    <Jumbotron/>
    <div class="main-container">
      <Comics/>
    </div>
  </main>
</template>

<script>
import Comics from './ComicsCard.vue'
import Jumbotron from './Jumbotron.vue'

export default {
  name: 'Main',
  components:{
    Comics,
    Jumbotron,
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