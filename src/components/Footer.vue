<template>
  <footer>
    <div class="footer-links">
      <div class="links">
        <ul class="sites">
          <h4>SITES</h4>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD magazine</a></li>
          <li><a href="#">DC kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC PowerVisa</a></li>
        </ul>
        <ul class="dc">
          <h4>DC</h4>
          <li><a href="#">Terms of use</a></li>
          <li><a href="#">Privacy policy (new)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshop</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
        <ul class="dc-comics">
          <h4>DC COMICS</h4>
          <li><a href="#">Character</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">Tv</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>
        <ul class="shop">
          <h4>SHOP</h4>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
      </div>
      <div class="footer-logo">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    <div class="social-wrapper">
      <div class="footer-social">
        <div class="footer-button">
          BOTTONE SIGN UP 
        </div>
        <div class="social-links">
          <div>SOCIAL LINKS</div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="scss">
@import '../assets/style/mixins.scss';

footer{
  height: 500px;
  background: #fff url(../assets/img/footer-bg.jpg) no-repeat center;
  background-size: cover;

  .footer-links{
    @include container();
    position: relative;
    display:flex;
    justify-content: space-between;
    height: 400px;
    .links{
      width: 40%;
      color: #fff;
      display: flex;
      flex-direction: column;
      flex-wrap: wrap-reverse;
      ul{
        display: flex;
        justify-content: flex-start;
        flex-direction: column;
        list-style: none;
        margin-top: 30px;
        h4{
          margin-bottom: 10px;
        }
        li a{
          text-decoration: none;
          color: grey;
        }
      }
    }
    .footer-logo{
      position: absolute;
      right: 0;
      top: -60px;
    }
  }
  .social-wrapper{
    height: 100px;
    position: relative;
    background-color: #303030;
    .footer-social{
      height: inherit;
      @include container();
      @include align();
      justify-content: space-between
    }
  }
}



</style>