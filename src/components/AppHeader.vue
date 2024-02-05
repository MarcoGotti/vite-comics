<script>
export default {
    name:'AppHeader'
}
</script>

<template>

<header>
    <div class="container">
      <div class="row justify_between">
        <div class="col">
          <img class="logo" src="/img/dc-logo.png" alt="">
        </div>
        <nav class="col">
            <ul class="main_menu">
              <li><a href="#">Characters</a></li>
              <li class="active"><a class="active" href="#">Comics</a></li>
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
    </div>
    <div class="wrapper">
        <img src="/img/jumbotron.jpg" alt="">
    </div>
  </header>

</template>



<style scoped>
header{
  background-color: aliceblue;

  & .logo{
    width: 80px;
    padding: 20px 0;
  }

  & nav {
    & .main_menu{
      list-style: none;
      display: flex;
      align-items: center;
      text-transform: uppercase;
      font-family: 'Roboto Condensed', sans-serif;
      font-weight: 600;
      font-size: 12px;

      & li.active{
          border-bottom: 5px solid var(--com-secondary);
        };

      & li{
        line-height: 120px;
        margin: 0 1rem;

        & a.active{
          color: var(--com-secondary);
        };
        
        & a {
          text-decoration: none; 
          color: var(--com-primary);       
        };
      }     
    }
  }

  & .wrapper{
    height: 300px;
    overflow-y: hidden;

    & img{
      width: 100%;
      display: block;
    }
  }
}

</style>