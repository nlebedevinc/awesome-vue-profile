<template>
  <div class="projectcard__component ">
    <div class="card">
      <img src="http://media.npr.org/assets/news/2009/10/27/facebook1_sq-17f6f5e06d5742d8c53576f7c13d5cf7158202a9.jpg?s=16" alt="" />
    </div>
  </div>
</template>

<script>
  export default {
    name: 'vue-project-card',
    components: {}
  }
</script>

<style lang="scss">
.projectcard__component {
  .card {
    width: 250px;
    min-height: 285px;
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
