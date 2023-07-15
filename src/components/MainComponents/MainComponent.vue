<script>
import LinksComponent from "./LinksComponent.vue";
import JumbotronComponent from "./JumbotronComponent.vue";
import CardComponent from "./CardComponent.vue";
export default{
  components:{
    LinksComponent,
    JumbotronComponent,
    CardComponent
  },
  data(){
    return {
      series: [
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
  }
 
}
</script>

<template>
  <main>
    <div class="main-top">
      <JumbotronComponent/>
      <!--end jumbotron-->
      <div class="container">
      <h2>Current series</h2>
      <div class="cards-container">
      <CardComponent 
        v-for="(currentSerie, index) in series"
        :key="index"
        :srcImg="currentSerie.thumb"
        :imgName="currentSerie.series"
      />
        <!--end card-->
      </div>
      <!--end cards container-->
      <div class="button-wrapper">
        <button>load more</button>
      </div>
      </div>
    </div>
    <LinksComponent/>
  </main>
</template>

<style lang="scss" scoped>

  main{
    background-color: #1C1C1C;
  }
  .container{
    color:#fff;
    h2{
      display: inline-block;
      padding: .3125rem .9375rem;
      transform: translateY(-50%);
      background-color: #0282F9;
    }
    .button-wrapper{
      text-align: center;
      button{
        padding: .625rem .9375rem;
        background-color: #0282F9;
        border: none;
        margin-bottom: 10px;   
        text-transform: uppercase;
        border:1px solid transparent;
        color:#fff; 
        cursor: pointer; 
        transition: border-color 200ms ease-in-out;
        &:hover{
          border-color:#fff;
        }
      }
    }
  }
  .cards-container{
    display: flex;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 1.25rem;
  }

</style>