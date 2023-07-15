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
</style>