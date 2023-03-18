<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <ul class="nav justify-content-center">
        <li class="nav-item">
          <RouterLink class="nav-link" to="/">Home</RouterLink>
        </li>
        <div class="vr"></div>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/about">About</RouterLink>
        </li>
        <div class="vr"></div>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/projects">Projects</RouterLink>
        </li>
      </ul>
    </div>
  </header>
  <RouterView />
</template>

<style>
@import '@/assets/base.css';

#app {
  margin: 0 auto;
  padding: 2rem 8rem;
  font-weight: normal;
}

header {
  line-height: 1.5;
  max-height: 10vh;
}

.nav .router-link-active {
  color: var(--bs-link-color);
}

.nav .nav-item {
  --bs-nav-link-color: grey;
}

</style>
