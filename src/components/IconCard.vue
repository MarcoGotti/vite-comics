<script>
    export default {
        name:'IconCard',
        props: {
            icon: Object
        }
    }
</script>


<template>

    <div class="card">
        <img :src="'/img/' + icon.image" alt="">
        <h3>{{ icon.text }}</h3>
    </div> 
    
</template>


<style scoped>
.card{
    height: 150px;
    display: flex;
    align-items: center;
    color: white;
    text-transform: uppercase;
    
    & img{
      height: 60px;
    };

    & img[src$="-visa.svg"]{
      width: 55px;
    }

    & h3{
      margin-left: 1rem;
      font-size: 10px;
    }
  }
</style>