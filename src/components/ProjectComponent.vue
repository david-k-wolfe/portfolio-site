<template class="project">
    <div class="container">
        <div class="grid">
            <div class="row">
                <div class="col justify-content-center">
                    <h2 class="project-title"> title </h2>
                </div>
            </div>
            <div class="row">
                <div class="col">
                    <img class="project-image rounded img-fluid" :src="imageSrc">
                </div>
            </div>
            <div class="row">
                <div class="col">
                    <par class="project-description">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                    </par>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
  setup() {
    const title="Test"
    const imageSrc="/src/assets/logo.svg"
    return {
        title,
        imageSrc
    }
  }
}

</script>

<style>

.project-title {
    margin: 0rem auto;
    display: flex;
    justify-content: center;
}

.project-image {
    margin: 0rem auto;
    max-height: 20rem;
}

.row {
    padding-bottom: 0.5rem
}
</style>


