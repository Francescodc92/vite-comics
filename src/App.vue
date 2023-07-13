<script>
import HeaderComponet from './components/HeaderComponet.vue';
import MainComponet from './components/MainComponet.vue';
export default {
  components: { HeaderComponet , MainComponet},
}
</script>

<template>
  <headerComponet/>
  <MainComponet/>
</template>

<style lang="scss">
 @use "assets/scss/main.scss";
</style>
