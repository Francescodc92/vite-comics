<script>
export default {
}
</script>

<template>
  <header>
    <div class="my-container">
      <div class="img-wrapper">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <ul>
        <li class="active">
          <a href="">
           characters
          </a>
        </li>
        <li>
          <a href="">
            comics
          </a>
        </li>
        <li>
          <a href="">
            movies
          </a>
        </li>
        <li>
          <a href="">
            tv
          </a>
        </li>
        <li>
          <a href="">
            games
          </a>
        </li>
        <li>
          <a href="">
            collecticles
          </a>
        </li>
        <li>
          <a href="">
            videos
          </a>
        </li>
        <li>
          <a href="">
            fans
          </a>
        </li>
        <li>
          <a href="">
            news
          </a>
        </li>
        <li>
          <a href="">
            shop
          </a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style lang="scss" scoped>
  @use "../assets/scss/main.scss";
  header{
    background-color:#fff ;
  }
  .my-container{
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .img-wrapper{
    width: 80px;
  }

  ul{
    height: 100%;
    display: flex;
    transition: color 200ms ease-in-out;
    li{
      height: 100%;
      margin-inline:10px ;
      display: flex;
      align-items: center;
      position: relative;
      text-align: center;
    }

    li a{
      color:#000;
      padding: .3125rem .3125rem;
      text-transform: uppercase;
      font-size: .875rem;
      font-weight: bold;
    }

    li::after{
      content: "";
      width: 100%;
      display: block;
      height: 4px;
      background: #0282F9;
      position: absolute;
      bottom:0;
      visibility: hidden;
      opacity: 0;
      transition: opacity 200ms ease-in-out;
    }
    li:hover, li.active a{
      color:#0282F9; 
    }

    li:hover::after, li.active::after{
      visibility: visible;
      opacity: 1;
    }
   
  }
  
</style>