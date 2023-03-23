<template>
    <div class="projects container">
        <div class="container text-center">
          <div class="row row-cols-3">
            <div class="col" v-for="project in projects">
              <ProjectComponent/>
            </div>
          </div>
        </div>
    </div>
</template>
  
<script>
import ProjectComponent from '../components/ProjectComponent.vue'

export default {
  setup () {
    const projects = [0, 1, 2, 4]
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
  