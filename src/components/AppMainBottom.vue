<script>

import IconCard from "./IconCard.vue";

export default {
    name: 'AppMainBottom',
    components: {
      IconCard
    },
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
            
            <IconCard :icon='icon'></IconCard>

          </div>         
        </div>
      </div> 
    </div>

</template>



<style scoped>

#main_bottom{
  background-color: var(--com-secondary);
}

</style>