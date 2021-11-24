<template>
  <header>
    <div class="head-wrapper">
      <div class="head-logo">
        <img src="../assets/img/dc-logo.png" alt="Logo Header">
      </div>
      <nav>
        <ul>
          <li><a href="#">Character</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">Tv</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Collectibles</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">Fans</a></li>
          <li><a href="#">News</a></li>
          <li><a href="#">Shop</a></li>
        </ul>
      </nav>
    </div>
    
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="scss">
@import '../assets/style/mixins.scss';

.head-wrapper {
  @include container();
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px; 
  .head-logo {
    width: 75px;
    height: 75px;
  }
}
ul{
  list-style: none;
  li {
    display: inline-block;
    margin: 0.8rem;
      a{
      text-decoration: none;
    }
  }
    
}
</style>