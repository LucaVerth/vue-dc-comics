<template>
  <main> 
    <div class="main-container">
      -->Content goes here 
    </div>
  </main>
</template>

<script>
export default {
  name: 'Main'
}
</script>

<style lang="scss">
@import '../assets/style/mixins.scss';

main{
  background-color: #000;
  color: #fff;
  .main-container{
    @include container();
    display:flex;
    align-items:center;
    min-height: 100px;
  }
}
</style>