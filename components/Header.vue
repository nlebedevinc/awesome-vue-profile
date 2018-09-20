<template>
  <div class="header__component ">
    <logo />
    <navigation />
  </div>
</template>

<script>
  import Logo from './Logo'
  import Navigation from './Navigation'
  export default {
    name: 'vue-header-logo',
    components: {
      Logo,
      Navigation
    }
  }
</script>

<style lang="scss">
.header__component {
  padding: 15px;
}
</style>
