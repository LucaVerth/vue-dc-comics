<template>
  <header>
    <div class="head-wrapper">
      <div class="head-logo">
        <img src="../assets/img/dc-logo.png" alt="Logo Header">
      </div>
      <nav>
        <ul>
          <li v-for="item in links" :key="item.id">
            <a href="#">{{item.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return {
      links: [
        {
          id: 1,
          url: '/',
          text: 'Character',
          active: false
        },
        {
          id: 2,
          url: '/',
          text: 'Comics',
          active: false
        },
        {
          id: 3,
          url: '/',
          text: 'Movies',
          active: false
        },
        {
          id: 4,
          url: '/',
          text: 'Tv',
          active: false
        },
        {
          id: 5,
          url: '/',
          text: 'Games',
          active: false
        },
        {
          id: 6,
          url: '/',
          text: 'Collectibles',
          active: false
        },
        {
          id: 7,
          url: '/',
          text: 'Videos',
          active: false
        },
        {
          id: 8,
          url: '/',
          text: 'Fans',
          active: false
        },
        {
          id: 9,
          url: '/',
          text: 'News',
          active: false
        },
        {
          id: 10,
          url: '/',
          text: 'Shop',
          active: false
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import '../assets/style/mixins.scss';

.head-wrapper {
  @include container();
  @include align();
  justify-content: space-between;
  height: 100px; 
  .head-logo {
    width: 75px;
    height: 75px;
  }
  ul{
    list-style: none;
    li {
      display: inline-block;
      margin: 0.8rem;
        a{
        text-decoration: none;
        color: #0D7CEC;
      }
    } 
  }
}

</style>