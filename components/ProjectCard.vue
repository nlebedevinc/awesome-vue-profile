<template>
  <div class="projectcard__component ">
    <nuxt-link class="navigation-link" to='/portfolio'>
      <div class="card">
        <div class="image-container">
          <img
            src="https://www.aks.ua/images/products/9956580dedf73c949ef4493b0032f1f4_large.jpg"
            alt=""/>
        </div>
        <div class="card-info">
          <h3>{{project.title}}</h3>
          <span>JavaScript | Node | CSS</span>
        </div>
      </div>
    </nuxt-link>
  </div>
</template>

<script>
  export default {
    name: 'vue-project-card',
    props: ['project'],
    components: {}
  }
</script>

<style lang="scss">
.projectcard__component {
  width: 345px;
  min-height: 350px;
  padding: 10px;

  .navigation-link {
    text-decoration: none;
    color: #000;
  }

  .card {
    border: 1px solid #eee;
    box-shadow: 0 10px 40px 0 rgba(133,157,183,.12);
    .card-info {
      padding: 20px;
    }
  }

  .image-container {
    max-height: 250px;
    overflow: hidden;
  }

  img {
    max-height: 300px;
  }
}
</style>
