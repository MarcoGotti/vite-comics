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
        transition: transform .5s;
        

/*       & :hover{
            filter: drop-shadow(0 0 10px var(--com-secondary));
            transform: scale(1.05);
      } */
      & .wrapper{
        height: 170px;
        overflow-y: hidden;

        & img {
         width: 100%;  
        };
      }

      & h6{
        margin-top: 1rem;
        text-transform: uppercase;
        text-align: left;
      }
    }

    & .card:hover{
            filter: drop-shadow(0 0 10px var(--com-secondary));
            transform: scale(1.05);
    }
   

</style>