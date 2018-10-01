<template>
  <section class="container">
    <header-logo />
    <div class="content">
      <project-list />
    </div>
  </section>
</template>

<script>
import HeaderLogo from '~/components/Header'
import ProjectList from '~/components/ProjectList'

export default {
  components: {
    HeaderLogo,
    ProjectList
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  padding: 15px;
  @media only screen and (min-device-width : 850px) {
    max-width: 950px;
    margin-top: 20px;
    margin-bottom: 20px;
  }

  .content {
    clear: both;
    padding: 50px 0;
  }
}
</style>
