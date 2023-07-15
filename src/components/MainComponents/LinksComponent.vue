<script>
  export default{
    methods:{
      getPath: (imgSrc)=> {
        return new URL(imgSrc, import.meta.url).href
      }
    },
    props:{
      linkSrc: String,
      linkText:String
    }
  }
</script>

<template>
  
  
  <li>
    <a href="#">
      <div class="img-wrapper">
        <img :src="getPath(linkSrc)" alt="">
      </div>
      {{linkText}}
    </a>
  </li>
  <!--end link-->
</template>

<style lang="scss" scoped>
  li{
    width: calc((100% - (1.25rem * 4)) / 5 );
    border: 1px solid transparent;
    transition: border-color 200ms ease-in-out;
    border-radius: 20px;
    a{
      display: flex;
      align-items: center;
      gap: .625rem;
      text-transform: uppercase;
      font-size: .875rem;
      padding: 20px 5px;
      color: #fff;
    }
    &:hover {
      border-color: #fff;
    }

  }
  .img-wrapper{
    width: 60px;
    height: 70px;
  }
</style>