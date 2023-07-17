<script>
export default {
  props:{
    href: String,
    text: String,
  }
}
</script>

<template>
    <li>
      <a :href="href">
        {{ text }}
      </a>
    </li>
</template>

<style lang="scss" scoped>
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;
  li{
        height: 100%;
        margin-inline:.3125rem ;
        display: flex;
        align-items: center;
        position: relative;
        text-align: center;
        & a{
          color: $dark-color;
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
          background: $primary-color;
          position: absolute;
          bottom:0;
          visibility: hidden;
          opacity: 0;
          transition: opacity 200ms ease-in-out;
        }
        &:hover a, &.active a{
        color: $primary-color ; 
        }
        &:hover::after, &.active::after{
          visibility: visible;
          opacity: 1;
        }
    }
</style>