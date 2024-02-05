<script>
    export default {
        name: 'AppFooterTop'
    }
</script>


<template>
    
    <div id="footer_top">
      <div class="container py_2 position_rel">
        <div class="row">
          <div class="col-">
            <h3>dc comics</h3>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h3>shop</h3>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="col-">
            <h3>dc</h3>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="col-">
            <h3>sites</h3>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>
        <img src="/img/dc-logo-bg.png" alt="">
      </div>
    </div>

</template>



<style scoped>
#footer_top{
  height: 370px;
  background-image: url('/img/footer-bg.jpg');
  background-size: 100% auto;
  overflow-y: hidden;
  color: var(--com-white);

  & h3{
    text-transform: uppercase;
    font-weight: 800;

  }

  & ul{
    list-style: none;
    margin: .75rem 0;

    & a{
      text-decoration: none;
      font-size: 12px;
      font-weight: 100;
      color: var(--com-white);
    }
  }

  & img{
    width: 560px;
    position: absolute;
    right: 0;
    top: -95px;
  }
}
</style>