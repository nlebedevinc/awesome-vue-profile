<template>
  <div class="projects__component ">
    <div class="container">
      <div v-for="project in list" :key="project.id">
        <project-card v-bind:project="project" />
      </div>
    </div>
  </div>
</template>

<script>
import ProjectCard from './ProjectCard'
export default {
  name: 'vue-project-list',
  props: ['list'],
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
