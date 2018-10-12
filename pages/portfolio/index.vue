<template>
  <section class="container">
    <header-logo />
    <div class="content">
      <project-list v-bind:list="projects"/>
    </div>
  </section>
</template>

<script>
import HeaderLogo from '~/components/Header'
import ProjectList from '~/components/ProjectList'
import { mapState } from 'vuex'
// import axios from 'axios'

export default {
  fetch ({ store }) {
    // return axios.get('http://localhost:3030/v1/projects/list')
    //   .then(res => {
    //     store.commit('projects', res.data)
    //   })
    store.commit('init', [
      {
        id: 1,
        title: 'First'
      },
      {
        id: 2,
        title: 'Second'
      },
      {
        id: 3,
        title: 'Third'
      }
    ])
  },
  computed: mapState([
    'projects'
  ]),
  components: {
    HeaderLogo,
    ProjectList
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  padding-top: 15px;
  padding-bottom: 15px;
  @media only screen and (min-device-width : 1200px) {
    max-width: 1035px;
    margin-top: 20px;
    margin-bottom: 20px;
  }

  .content {
    clear: both;
    padding: 50px 0;
  }
}
</style>
