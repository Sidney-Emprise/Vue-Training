<script setup lang="ts">
import TheWelcome from '../components/AboutPage/TheWelcome.vue'
</script>


<template>
  <div class="about">
    <TheWelcome />
  </div>
</template>



<style>
@media (min-width: 1024px) {
  .about {
    min-height: 50vh;
    /* display: flex;
    align-items: center;
    padding: inherit; */
  }
}
</style>
