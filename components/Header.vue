<template>
  <div class="header__component ">
    <logo class="header-logo"/>
    <div class="header-navigation">
      <navigation />
    </div>
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
  .header-logo {
    float: left;
  }
  .header-navigation {
    margin-top: 15px;
    float: right;
  }
}
</style>
