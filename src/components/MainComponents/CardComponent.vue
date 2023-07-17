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
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;
  .card{
    width: calc((100% - (20px * 5)) / 6 );
    padding-inline:.625rem;
    padding-block: .625rem ;
    margin-bottom: 30px;
    border: 1px solid transparent;
    border-radius: 15px;
    transition: border-color 200ms ease-in-out;
    
    a{
      color: $primary-text-color;
    }
    
    &:hover{
      border-color: $primary-text-color;
    }
    .img-wrapper{
      width: 100%;
      height: 250px;
      img{
        width: 100%;
        height: 100%;
        object-fit:contain;
      }
    }
    h3{
      font-size: .75rem;
      font-weight: normal;
      text-transform: uppercase;
    }
  }
</style>