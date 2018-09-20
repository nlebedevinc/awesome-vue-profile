<template>
  <section class="container">
    <header-logo />
  </section>
</template>

<script>
import HeaderLogo from '~/components/Header'

export default {
  components: {
    HeaderLogo
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  padding: 15px;
  @media only screen and (min-device-width : 850px) {
    max-width: 850px;
    margin-top: 20px;
    margin-bottom: 20px;
  }
}
</style>
