<script>
import HeaderComponet from './components/HeaderComponet.vue';
import MainComponet from './components/MainComponet.vue';
import FooterComponet from './components/FooterComponent.vue'
export default {
  components: { HeaderComponet , MainComponet, FooterComponet},
}
</script>

<template>
  <headerComponet/>
  <MainComponet/>
  <FooterComponet/>
</template>

<style lang="scss">
 @use "assets/scss/main.scss" as *;// da usare sempre per non scordarlo  in caso di utilizzo di variabili 
</style>
