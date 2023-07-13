<script></script>

<template>
 <footer>
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
  </div>

 </footer>
</template>

<style lang="scss" scoped>
  @use "../assets/scss/main.scss";
  footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
  }
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
</style>