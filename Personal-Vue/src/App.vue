<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div>
    <header>
      <img alt="Seemly Sand logo" class="logo" src="./assets/SeemlySandLogo.svg" width="225" height="225" /> 

      <div class="wrapper">
        <HelloWorld name="Sidney R Sanders" msg = "Software Developer II with Emprise Technologies"/>
      </div>
      <nav>
        <RouterLink to="/">Go to Home</RouterLink>
        <RouterLink to="/about">Go to About</RouterLink>
      </nav>
    </header>

    <RouterView />
    <TheWelcome />

  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
    justify-content: center;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
