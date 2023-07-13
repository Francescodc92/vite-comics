<script></script>

<template>
 <footer>
   <div class="footer-top">
      <div class="container">
      <div class="footer-section">
        <h3 class="title">DC comics</h3>
        <ul>
          <li class="list-item">
            <a href="">
              Characters
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              Ccomics
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              Movies
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
             tv
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              Games
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              videos
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              news
            </a>
          </li>
          <!--end list item-->
        </ul>
        <!--end link list -->
  
        <h3 class="title">
          Shop
        </h3>
        <ul>
          <li class="list-item">
            <a href="">shop dc</a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">shop dc Collectibles</a>
          </li>
          <!--end list item-->
        </ul>
        <!--end link list-->
      </div>
      <!--end section footer top-->
      <div class="footer-section">
        <h3 class="title">DC</h3>
        <ul>
          <li class="list-item">
            <a href="">
              Terms of use
            </a>
          </li>
          <li class="list-item">
            <a href="">
              privacy policy(New)
            </a>
          </li>
          <li class="list-item">
            <a href="">
             ad choices
            </a>
          </li>
          <li class="list-item">
            <a href="">
             advertising
            </a>
          </li>
          <li class="list-item">
            <a href="">
             jobs
            </a>
          </li>
          <li class="list-item">
            <a href="">
             subscriptions
            </a>
          </li>
          <li class="list-item">
            <a href="">
             talent workshops
            </a>
          </li>
          <li class="list-item">
            <a href="">
             CPSC Certigicates
            </a>
          </li>
          <li class="list-item">
            <a href="">
             Ratings
            </a>
          </li>
          <li class="list-item">
            <a href="">
             Shop Help
            </a>
          </li>
          <li class="list-item">
            <a href="">
             contact us
            </a>
          </li>
  
        </ul>
        <!--end link list -->
      </div>
      <!--end section footer top-->
      <div class="footer-section">
        <h3 class="title">DC comics</h3>
           <ul>
          <li class="list-item">
            <a href="">
              Dc
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              MAD Magazine
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              DC Kids
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
             DC Universe
            </a>
          </li>
          <!--end list item-->
          <li class="list-item">
            <a href="">
              DC Power Visa
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
              <img src="../assets/img/footer-facebook.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../assets/img/footer-twitter.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../assets/img/footer-youtube.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../assets/img/footer-pinterest.png" alt="">
            </a>
          </li>
          <li>
            <a class="link" href="">
              <img src="../assets/img/favicon.ico" alt="">
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
  @use "../assets/scss/main.scss";
  .footer-top{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    .container{
      height: 100%;
      position: relative;
      display: flex;
      padding: 30px;
      gap: 30px;
    }
    .container::after{
      content: '';
      display: block;
      width: 40%;
      height: 100%;
      background-image: url(../assets/img/dc-logo-bg.png);
      background-position: center;
      background-size: cover;
      position: absolute;
      right: 0;
      top: 0;
    }
  }

  .title{
    text-transform: uppercase;
    color: #fff;
    margin-top: 10px;
  }

  .list-item{
    margin: 5px 0;
     a{
      font-size: 13px;
      color:#8f8d8d;
      padding: 10px 0;
    }
    &:hover a{
      text-decoration: underline;
    }
  }
  .footer-bottom{
    background-color: #303030;
    .container{
      padding: 30px 0;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    .section-left{
      button{
        font-size: 1.125rem;
        background: transparent;
        border: 2px solid #0282F9;
        color:#fff;
        padding: 10px 15px;
        text-transform: uppercase;
      }
    }
    .section-right{
      display: flex;
      align-items: center;
      gap: .9375rem;
      .title{
        color: #0282F9;
      }
      .social-links {
        display: flex;
        gap: .9375rem;
        .link {
          width: 40px;
          height: 40px;
          display: block;
        }
      }
    }
  }
</style>