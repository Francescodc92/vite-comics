<script>
import CardsComponet from "./CardsComponet.vue";
export default{
  components:{
    CardsComponet
  }
}
</script>

<template>
  <main>
    <div class="main-top">
      <div class="container">
      <h1>Content goas here</h1>
      </div>
    </div>
    <CardsComponet/>
  </main>
</template>

<style lang="scss" scoped>
  @use "../assets/scss/main.scss";
  .container{
    padding: 50px 0;
    color:#fff;
  }
 
</style>