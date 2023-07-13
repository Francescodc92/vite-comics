<script></script>

<template>
  <main>
    <div class="main-top">
      <div class="container">
      <h1>Content goas here</h1>
      </div>
    </div>
    <div class="main-bottom">
      <div class="container">
        <ul>
          <li>
            <a href="">
              <div class="img-wrapper">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
              </div>
              digital comics
            </a>
          </li>
          <!--end link-->
          <li>
            <a href="">
              <div class="img-wrapper">
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
              </div>
              dc merchandise
            </a>
          </li>
          <!--end link-->
          <li>
            <a href="">
              <div class="img-wrapper">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
              </div>
              subscription
            </a>
          </li>
          <!--end link-->
          <li>
            <a href="">
              <div class="img-wrapper">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
              </div>
              comic shop locator
            </a>
          </li>
          <!--end link-->
          <li>
            <a href="">
              <div class="img-wrapper">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
              </div>
              dc power visa
            </a>
          </li>
          <!--end link-->
        </ul>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
  @use "../assets/scss/main.scss";
  .container{
    padding: 50px 0;
    color:#fff;
  }
  .main-bottom{
    background-color:#0282F9;
    padding: 0 30px;
  }

  ul{
    display: flex;
    justify-content: space-between;
    align-items: center;
    li{
      border: 1px solid transparent;
      transition: color 200ms ease-in-out;
      border-radius: 20px;
      a{
        display: flex;
        align-items: center;
        gap: .625rem;
        text-transform: uppercase;
        font-size: .875rem;
        color: #fff;
        padding: 20px 30px;
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

</style>