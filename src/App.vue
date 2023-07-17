<script>
import HeaderComponent from './components/HeaderComponents/HeaderComponent.vue';
import MainComponent from './components/MainComponents/MainComponent.vue';
import FooterComponent from './components/FooterComponents/FooterComponent.vue'
export default {
  components: { HeaderComponent , MainComponent, FooterComponent},
}
</script>

<template>
  <headerComponent/>
  <MainComponent/>
  <FooterComponent/>
</template>

<style lang="scss">
 @use "assets/scss/main.scss" as *;
 @use "assets/scss/partials/variables.scss" as *;
</style>
