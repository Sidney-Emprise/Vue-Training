<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/SeemlySandLogo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="Sidney Sanders" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/strategy">Strategy</RouterLink>
        <RouterLink to="/help">Help</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  /* margin: 0 auto 2rem; */
}

nav {
  width: 100%;
  font-size: 14px;
  text-align: left;
  margin-top: 1rem;
  margin-bottom: 2rem;
  margin-left: -1rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: inline-flex;
    place-items: center;
    justify-content: left;
    gap: 2rem;
  }

  .logo {
    margin: 0rem 0rem 3rem 0rem;
    border-radius: 50%;
    border: 2px solid rgb(149, 69, 255);
  }

  header .wrapper {
    display: inline-flex;
    place-items: center;
    flex-wrap: wrap;
    justify-content: left;
    flex-direction: column;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
