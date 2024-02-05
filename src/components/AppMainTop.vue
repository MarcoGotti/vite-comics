<script>
export default{
    name: 'AppMainTop',
    data(){
      return{
        comics:[
          {
            "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
            "price": "$19.99",
            "series": "Action Comics",
            "type": "comic book",
          },
          {
            "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
            "price": "$3.99",
            "series": "American Vampire 1976",
            "type": "comic book",
          },
          {
            "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
            "price": "$16.99",
            "series": "Aquaman",
            "type": "graphic novel",
          },
          {
            "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
            "price": "$2.99",
            "series": "Batgirl",
            "type": "comic book",
          },
          {
            "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
            "price": "$3.99",
            "series": "Batman",
            "type": "comic book",
          },
          {
            "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
            "price": "$2.99",
            "series": "Batman Beyond",
            "type": "comic book",
          },
          {
            "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
            "price": "$3.99",
            "series": "Batman/Superman",
            "type": "comic book",
          },
          {
            "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
            "price": "$4.99",
            "series": "Batman/Superman Annual",
            "type": "comic book",
          },
          {
            "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
            "price": "$5.99",
            "series": "Batman: The Joker War Zone",
            "type": "comic book",
          },
          {
            "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
            "price": "$6.99",
            "series": "Batman: Three Jokers",
            "type": "comic book",
          },
          {
            "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
            "price": "$4.99",
            "series": "Batman: White Knight Presents: Harley Quinn",
            "type": "comic book",
          },
          {
            "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
            "price": "$16.99",
            "series": "Catwoman",
            "type": "graphic novel",
          },

        ]
      }
    },
}
</script>

<template>

    <div id="main_top">

      <div class="label">
          current series
      </div>
      
      <div class="container">
        <div class="row">
          <div class="col-2" v-for="comic in comics">

            <div class="card">
              <div class="wrapper">
                <img :src="comic.thumb" alt="">
              </div>            
              <h6>{{ comic.series }}</h6>
            </div>

            
          </div>
        </div>
      </div>      
    </div>

</template>



<style scoped>

#main_top{
  color: var(--com-white);
  min-height: 150px;
  padding: 2rem 0;
  position: relative;

  & .label{
      position: absolute;
      top: -30px;
      left: 180px;
      background-color: var(--com-secondary);
      padding: .75rem;
      text-transform: uppercase;
      font-weight: 600;
    }

  & .row{
    flex-wrap: wrap;
    row-gap: 2rem;

    & .card {
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
  } 
}

</style>