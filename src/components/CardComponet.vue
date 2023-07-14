<script>
export default{
  props:{
    srcImg: String,
    imgName : String,
  }
}
</script>


<template>
    <div href="" class="card">
      <a href="">
        <div class="img-wrapper">
          <img :src="srcImg" :alt="imgName">
        </div>
        <h3>{{imgName}}</h3>
      </a>
    </div>
</template>

<style lang="scss" scoped>
  .card{
    width: calc((100% - 4%) / 6 );
    height: 100%;
    padding-inline:.625rem;
    padding-top: .625rem ;
    margin-bottom: 30px;
    border: 1px solid transparent;
    border-radius: 15px;
    transition: border-color 200ms ease-in-out;
    
    a{
      color: #fff;
    }
    
    &:hover{
      border-color: #fff;
    }
    .img-wrapper{
      width: 100%;
      height: 250px;
      img{
        min-width: 100%;
        min-height: 100%;
        object-fit:contain;
      }
    }
    h3{
      font-size: .9375rem;
      font-weight: normal;
      text-transform: uppercase;
      padding: 10px 0;
    }
  }
</style>