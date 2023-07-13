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
            link
          </a>
        </li>
        <li>
          <a href="">
            link
          </a>
        </li>
        <li>
          <a href="">
            link
          </a>
        </li>
        <li>
          <a href="">
            link
          </a>
        </li>
        <li>
          <a href="">
            link
          </a>
        </li>
        <li>
          <a href="">
            link
          </a>
        </li>
        <li>
          <a href="">
            link
          </a>
        </li>
        <li>
          <a href="">link</a>
        </li>
        <li>
          <a href="">link</a>
        </li>
        <li>
          <a href="">link</a>
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
    }
    li a::after{
      content: "";
      width: 100%;
      display: block;
      height: 2px;
      background: #0282F9;
      position: absolute;
      bottom:0;
      visibility: hidden;
      opacity: 0;
      transition: opacity 200ms ease-in-out;
    }
    li:hover a{
      color:#0282F9;
    }

    li:hover a::after{
      visibility: visible;
      opacity: 1;
    }
    li.active a::after{
      visibility: visible;
      opacity: 1;
    }
    a{
      padding: .3125rem 0;
    }
  }
  
</style>