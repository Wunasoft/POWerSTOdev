<script setup lang="ts">
// import { RouterLink, RouterView } from 'vue-router'
 import {RouterLink} from 'vue-router'
import HeaderLogo from './components/modules/HeaderLogo.vue';
</script>

<template>
  <HeaderLogo/>
  <nav>
    <RouterLink to="/">Home</RouterLink>
  </nav>
 
</template>

<style scoped>


  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }

</style>
