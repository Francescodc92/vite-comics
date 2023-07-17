<script>
import HeaderLinksComponent from './HeaderLinksComponent.vue';
export default {
  components:{
    HeaderLinksComponent
  },
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
       <HeaderLinksComponent 
       :class="link.isActive ? 'active' : ''"
        v-for="(link, index) in linksMenu" 
        :key="index"
        :href="link.linkHref"
        :text="link.linkText"
        />
        <!--end link-->
      </ul>
    </div>
  </header>

</template>

<style lang="scss" scoped>
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;
  header{
    background-color: $primary-text-color ;
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
      
  }
  
</style>