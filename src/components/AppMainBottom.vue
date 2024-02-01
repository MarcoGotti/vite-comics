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
      <div class="container pl_2">
        <div class="row">
          
          <div  v-for="icon in iconList" class="col grow_1">
            <div class="card">
              <img :src="'/img/' + icon.image" alt="">
              <h3>{{icon.text}}</h3>
            </div>           
          </div>
          
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

    & img[src$="-visa.svg"]{
      width: 60px;
    }

    & h3{
      margin-left: 1rem;
      font-size: 12px;
    }
  }
}

</style>