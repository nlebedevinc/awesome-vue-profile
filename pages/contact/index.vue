<template>
  <section class="container">
    <header-logo />
    <div class="content">
    </div>
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
.content {
  border: 1px solid #000;
  height: 20px;
}

</style>