<template>
  <div class="main-information__component">
    <particles
      :clickEffect="false"
      color="#dedede" />

      <div class="main-information-card">
        <h1>Nikolay Lebedev</h1>
        <h2>@nlebedevinc</h2>

        <div class="main-information-card-icons">
          <a href="https://github.com/nlebedevinc">
            <icon name="brands/github" scale="2" />
          </a>

          <a href="">
            <icon name="brands/medium" scale="2" />
          </a>

          <a href="">
            <img src="https://d2fltix0v2e0sb.cloudfront.net/dev-badge.svg" alt="Nikita Sobolev's DEV Profile" height="30" width="30" />
          </a>

          <a href="">
            <icon name="microphone-alt" scale="2" />
          </a>
        </div>
      </div>
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
  </div>
</template>

<script>
import Particles from './Particles'

export default {
  components: {
    // Internal:
    Particles
  }
}
</script>

<style lang="scss">
.main-information__component {
  background-color: #222;
  height: 100vh;
  position: relative;

  display: flex;
  justify-content: center;
  align-items: center;

  a, a:hover, a:active {
    color: black;
    text-decoration: none;
  }

  #particles-js {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;

    canvas {
      height: 99% !important;
    }
  }

  .main-information-card {
    background-color: #f3f3f3;

    padding: 50px;
    text-align: center;
    z-index: 2;

    .main-information-card-icons {
      margin-top: 30px;

      svg,
      img {
        margin: 10px;
      }
    }
  }
  .main-navigation-card {
    position: absolute;
    bottom: 0;
    margin-bottom: 60px;
  }
}
</style>
