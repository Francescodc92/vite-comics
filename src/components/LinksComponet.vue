<script>
export default{
  data(){
    return {
      cardsContent: [
        {
          img:'../assets/img/buy-comics-digital-comics.png',
          text: 'digital comics'
        },
        {
          img:'../assets/img/buy-comics-merchandise.png',
          text: 'dc merchandise'
        },
        {
          img:'../assets/img/buy-comics-subscriptions.png',
          text: 'subscription'
        },
        {
          img:'../assets/img/buy-comics-shop-locator.png',
          text: 'comic shop locator'
        },
        {
          img:'../assets/img/buy-dc-power-visa.svg',
          text: 'dc power visa'
        }
      ]
    }
  },
  methods:{
    getPath: (imgSrc)=> {
      return new URL(imgSrc, import.meta.url).href
    }
  }
}
</script>

<template>
  <div class="main-bottom">
      <div class="container">
        <ul>
          <li v-for="(card, index) in cardsContent" :key="index">
            <a href="">
              <div class="img-wrapper">
                <img :src="getPath(card.img)" alt="">
              </div>
              {{card.text}}
            </a>
          </li>
          <!--end link-->
        </ul>
      </div>
  </div>
</template>

<style lang="scss" scoped>
  .container{
    padding: 50px 0;
    color:#fff;
  }
 .main-bottom{
    background-color:#0282F9;
    padding: 0 30px;
    ul{
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 1.25rem;
      li{
        border: 1px solid transparent;
        transition: border-color 200ms ease-in-out;
        border-radius: 20px;
        a{
          display: flex;
          align-items: center;
          gap: .625rem;
          text-transform: uppercase;
          font-size: .875rem;
          color: #fff;
          padding: 20px 10px;
        }
        &:hover {
          border-color: #fff;
        }
  
      }
    }
    .img-wrapper{
      width: 60px;
      height: 70px;
    }
  }
</style>