<template>
  <div class="main-navigation-card">
    <nuxt-link to='/portfolio'>
      <span>Portfolio</span>
    </nuxt-link>

    <nuxt-link to='/resume'>
      <span>Resume</span>
    </nuxt-link>

    <nuxt-link to='/contact'>
      <span>Contact</span>
    </nuxt-link>
  </div>
</template>

<script>
  export default {
    name: 'vue-navigation'
  }
</script>