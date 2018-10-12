<template>
  <div class="navigation__component ">
    <nuxt-link class="navigation-link" to='/portfolio'>
      <span v-bind:class="{ 'white-text': whiteLabel, 'basic-text': !whiteLabel}">Portfolio</span>
    </nuxt-link>

    <nuxt-link class="navigation-link" to='/resume'>
      <span v-bind:class="{ 'white-text': whiteLabel, 'basic-text': !whiteLabel}">Resume</span>
    </nuxt-link>

    <nuxt-link class="navigation-link" to='/contact'>
      <span v-bind:class="{ 'white-text': whiteLabel, 'basic-text': !whiteLabel}">Contact</span>
    </nuxt-link>
  </div>
</template>

<script>
  export default {
    name: 'vue-navigation',
    props: ['whiteLabel']
  }
</script>

<style lang="scss">
.navigation__component {
  padding-top: 15px;
  padding-bottom: 15px;

  .navigation-link {
    padding-right: 15px;
    padding-left: 15px;
    text-decoration: none;
    text-transform: uppercase;

    .white-text {
      color: #fff;
    }

    .basic-text {
      color: #000;
    }
  }
}
</style>
