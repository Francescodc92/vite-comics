<script>
export default{
  data(){
    return {
      dcComixLinks: [
        'Characters',
        'Comics',
        'Movies',
        'Tv',
        'Games',
        'Videos',
        'News',
      ],
      shop: [
        'Shop Dc',
        'Shop Dc Collectibles'
      ], 
      DC: [
        'Terms of use',
        'privacy policy(New)',
        'ad choices',
        'advertising',
        'jobs',
        'subscriptions',
        'talent workshops',
        'CPSC Certigicates',
        'Ratings',
        'Shop Help',
        'contact us',
      ],
      DcComics:[
        'DC',
        'MAD Magazine',
        'DC kids',
        'DC Universe',
        'DC  Power Visa',
      ]
    }
  }
}
</script>

<template>
 <footer>
   <div class="footer-top">
      <div class="container">
      <div class="footer-section">
        <h3 class="title">DC comics</h3>
        <ul>
          <li class="list-item" v-for="(link, index) in dcComixLinks" :key="index">
            <a href="">
              {{ link }}
            </a>
          </li>
          <!--end list item-->
        </ul>
        <!--end link list -->
  
        <h3 class="title">
          Shop
        </h3>
        <ul>
          <li class="list-item" v-for="(link, index) in shop" :key="index">
            <a href="">{{ link }}</a>
          </li>
          <!--end list item-->
        </ul>
        <!--end link list-->
      </div>
      <!--end section footer top-->
      <div class="footer-section">
        <h3 class="title">DC</h3>
        <ul>
          <li class="list-item" v-for="(link, index) in DC" :key="index">
            <a href="">
              {{ link }}
            </a>
          </li>
        </ul>
        <!--end link list -->
      </div>
      <!--end section footer top-->
      <div class="footer-section">
        <h3 class="title">DC comics</h3>
        <ul>
          <li class="list-item" v-for="(link, index) in DcComics" :key="index">
            <a href="">
              {{ link }}
            </a>
          </li>
          <!--end list item-->
        </ul>
        <!--end link list -->
      </div>
      <!--end section footer top-->
    </div>
    <!--end footer top-->
  </div>
  <div class="footer-bottom">
    <div class="container">
      <div class="section-left">
        <button>
          Sign-up now!
        </button>
      </div>
      <div class="section-right">
        <h3 class="title">follow us</h3>
        <ul class="social-links">
          <li>
            <a class="link" href="">
              <img src="../../assets/img/footer-facebook.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../../assets/img/footer-twitter.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../../assets/img/footer-youtube.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../../assets/img/footer-pinterest.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../../assets/img/footer-periscope.png" alt="">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>  
  <!--end footer bottom-->

 </footer>
</template>

<style lang="scss" scoped>
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;
  .footer-top{
    background-image: url(../../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    .container{
      height: 100%;
      position: relative;
      display: flex;
      padding: 30px;
      gap: 30px;
      background-image: url(../../assets/img/dc-logo-bg.png);
      background-position: right;
      background-size: 45%;
      background-repeat: no-repeat;
    }
  
  }

  .title{
    text-transform: uppercase;
    color: $primary-text-color ;
    margin-top: 10px;
  }

  .list-item{
    margin: 5px 0;
     a{
      font-size: 13px;
      color: $links-footer-color ;
      padding: 10px 0;
    }
    &:hover a{
      text-decoration: underline;
    }
  }
  .footer-bottom{
    background-color: $footer-bg-color ;
    .container{
      padding-block: 30px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    .section-left{
      button{
        font-size: 1.125rem;
        background: transparent;
        border: 2px solid $primary-color ;
        color: $primary-text-color;
        padding: 10px 15px;
        text-transform: uppercase;
        transition: background-color 200ms ease-in-out;
        cursor: pointer;
        &:hover{
          background-color: $primary-color ;
        }
      }
    }
    .section-right{
      display: flex;
      align-items: center;
      gap: .9375rem;
      .title{
        color: $primary-color ;
      }
      .social-links {
        display: flex;
        gap: .9375rem;
        .link {
          width: 40px;
          height: 40px;
          display: block;
          border: 2px solid transparent;
          border-radius:50%;
          transition: border-color 200ms ease-in-out;
          &:hover{
            border-color: $primary-text-color ;
          }
        }
      }
    }
  }
</style>