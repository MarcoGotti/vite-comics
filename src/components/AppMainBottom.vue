<script>
export default {
    name: 'AppMainBottom',
    data(){
        return{
            iconList:[
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    text: 'subscrition'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },
            ]
        }
        
    }
}
</script>

<template>

    <div id="main_bottom">
      <div class="container">
        <div class="row">
          
          <div  v-for="icon in iconList" class="col grow_1">
            <div class="card">
              <img :src="'/img/' + icon.image" alt="">
              <h3>{{icon.text}}</h3>
            </div>           
          </div>
          
          <!-- <div class="col grow_1">
            <div class="card">
              <img src="/img/buy-comics-digital-comics.png" alt="">
              <h3>digital comics</h3>
            </div>           
          </div>
          <div class="col grow_1">
            <div class="card">
              <img src="/img/buy-comics-merchandise.png" alt="">
              <h3>dc merc
                handise</h3>
            </div>           
          </div>
          <div class="col grow_1">
            <div class="card">
              <img src="/img/buy-comics-subscriptions.png" alt="">
              <h3>subscription</h3>
            </div>           
          </div>
          <div class="col grow_1">
            <div class="card">
              <img src="/img/buy-comics-shop-locator.png" alt="">
              <h3>comic shop locator</h3>
            </div>           
          </div>
          <div class="col grow_1">
            <div class="card">
              <img src="/img/buy-dc-power-visa.svg" alt="">
              <h3>dc power visa</h3>
            </div>           
          </div> -->
        </div>
      </div> 
    </div>

</template>



<style scoped>

#main_bottom{
  background-color: var(--com-secondary);

  & .card{
    height: 150px;
    display: flex;
    align-items: center;
    color: white;
    text-transform: uppercase; 
    
    & img{
      height: 60px;
    };

    & h3{
      margin-left: 1rem;
      font-size: 12px;
    }
  }
}

</style>