<template>
    <div class="projects container">
        <div class="grid">
          <div class="row" v-for="project in projects">
            <ProjectComponent/>
          </div>
        </div>
    </div>
</template>
  
<script>
import ProjectComponent from '../components/ProjectComponent.vue'

export default {
  setup () {
    const projects = [0, 1, 2]
    return { projects }

  },
  components: {
    ProjectComponent
  }
}

</script>

<style>
@media (min-width: 1024px) {
  .projects {
    min-height: 100vh;
    display: flex;
    align-items: center;
    padding-top: 2rem;
  }
}
</style>
  