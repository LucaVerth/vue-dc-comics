<template>
  <div class="jumbotron">
   <img class="jumbo-image" :src="require('../assets/img/jumbotron.jpg')" alt="">
  </div>
</template>

<script>

export default {
  name: 'Jumbotron',
}
</script>

<style lang="scss">
.jumbotron{
  height: 400px;
  .jumbo-image{
    width: 100%;
    max-height: 100%;
    object-fit: cover;
    object-position: center top;
  }
}
</style>