<template>
  <section class="container">
    <header-logo />
    <div class="content">
      <span>Skdfsiojfiosdfosfjosoif</span>
      <div class="project-container">
        <div class="project-card">
          <img src="http://media.npr.org/assets/news/2009/10/27/facebook1_sq-17f6f5e06d5742d8c53576f7c13d5cf7158202a9.jpg?s=16" alt="" />
        </div>

        <div class="project-card">
          <img src="http://media.npr.org/assets/news/2009/10/27/facebook1_sq-17f6f5e06d5742d8c53576f7c13d5cf7158202a9.jpg?s=16" alt="" />
        </div>

        <div class="project-card">
          <img src="http://media.npr.org/assets/news/2009/10/27/facebook1_sq-17f6f5e06d5742d8c53576f7c13d5cf7158202a9.jpg?s=16" alt="" />
        </div>

        <div class="project-card">
          <img src="http://media.npr.org/assets/news/2009/10/27/facebook1_sq-17f6f5e06d5742d8c53576f7c13d5cf7158202a9.jpg?s=16" alt="" />
        </div>

        <div class="project-card">
          <img src="http://media.npr.org/assets/news/2009/10/27/facebook1_sq-17f6f5e06d5742d8c53576f7c13d5cf7158202a9.jpg?s=16" alt="" />
        </div>
      </div>
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

  .project-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  .project-card {
    width: 300px;
    min-height: 250px;
    border: 1px solid gray;
    padding: 10px;
    margin: 10px;
  }

  img {
    border-radius: 50%;
    width: 70px;
    margin: 10px;
  }
}
</style>
