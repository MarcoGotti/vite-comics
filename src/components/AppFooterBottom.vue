<script>
    export default {
        name: 'AppFooterBottom'
    }
</script>

<template>
 
 <div id="footer_bottom">
      <div class="container d_flex justify_between">
        <div class="action">
          sign-up now!
        </div>
        <div class="social d_flex">
          <h2 class="text">follow us</h2>
          <div class="icons">

            <!-- "...caricamento non riuscito ... bloccato a causa del tipo MIME non consentito (“image/gif”)..."
            <img src="/img/footer-facebook.png" alt="">
            <img src="/img/footer-twitter.png" alt=""> -->
            
            <img src="/img/footer-periscope.png" alt="">
            <img src="/img/footer-pinterest.png" alt="">
            <img src="/img/footer-youtube.png" alt="">
            
          </div>
        </div>
      </div>
    </div>

</template>

<style scoped>
#footer_bottom{
  height: 110px;
  background-color: var(--com-dark);

  & .container{
    height: 100%;
    align-items: center;

    & .action{
    text-transform: uppercase;
    color: var(--com-white);
    border: 3px solid var(--com-secondary);
    padding: 1rem;
  };

  & .social{
    align-items: center;
    
    & h2{
      color: var(--com-secondary);
      text-transform: uppercase;
      font-family: 'Roboto Condensed', sans-serif;
      font-weight: 600;
      font-size: 20px;
    };
    & .icons{
      margin-left: 1rem;

      & img{
        margin-left: 1rem;
      }
    }
  }
  }

  
}
</style>