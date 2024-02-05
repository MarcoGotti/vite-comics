<script>
export default {
   name: 'ComicCard',
   props: {
      comic: Object
    }, 
}
</script>

<template>
<div class="col-2">
    <div class="card">
        <div class="wrapper">
            <img :src="comic.thumb" alt="">
        </div>            
        <h6>{{ comic.series }}</h6>
    </div>           
</div>  
</template>



<style scoped>


    .card {
      & .wrapper{
        height: 170px;
        overflow-y: hidden;

        & img {
         width: 100%;  
        };
      }

      & h6{
        text-transform: uppercase;
      }
    }
   

</style>