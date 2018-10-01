<template>
  <div class="projects__component ">
    <div class="container">
      <project-card />
      <project-card />
      <project-card />
      <project-card />
      <project-card />
      <project-card />
      <project-card />
      <project-card />
      <project-card />
    </div>
  </div>
</template>

<script>
import ProjectCard from './ProjectCard'
export default {
  name: 'vue-project-list',
  components: {
    ProjectCard
  }
}
</script>

<style lang="scss">
.projects__component {
  .container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>
