<script>
export default {
  data(){
   return{
     linksMenu: [
        {
          linkHref:'#',
          linkText: 'characters',
          isActive:true,
        },
        {
          linkHref:'#',
          linkText: 'comics',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: 'movies',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: 'tv',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: 'games',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: 'collecticles',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: 'videos',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: 'fans',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: 'news',
          isActive:false,
        },
        {
          linkHref:'#',
          linkText: ' shop',
          isActive:false,
        },
    ]
   } 
  }
}
</script>

<template>
  
  <header>
    <div class="container">
      <div class="img-wrapper">
        <a href="">
          <img src="../../assets/img/dc-logo.png" alt="">
        </a>
      </div>
      <ul>
        <li :class="link.isActive ? 'active' : ''" v-for="(link, index) in linksMenu" :key="index">
          <a :href="link.linkHref">
           {{ link.linkText }}
          </a>
        </li>
        <!--end link-->
      </ul>
    </div>
  </header>

</template>

<style lang="scss" scoped>
  header{
    background-color:#fff ;
  }
  .container{
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
        margin-inline:.3125rem ;
        display: flex;
        align-items: center;
        position: relative;
        text-align: center;
        & a{
          color:#000;
          padding: 1.25rem .3125rem;
          text-transform: uppercase;
          font-size: .75rem;
          font-weight: bold;
          transition: color 200ms ease-in-out;
        }

        &::after{
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
        &:hover a, &.active a{
        color:#0282F9; 
        }
        &:hover::after, &.active::after{
          visibility: visible;
          opacity: 1;
        }
    }
  }
  
</style>