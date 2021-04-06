<template>
  <header class="header-container">
    <NuxtLink to="/" class="logo">
      <Logo />
    </NuxtLink>
    <NavigationBar id="navigation-bar" />
    <LightOrDark id="light-or-dark" />
  </header>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style scoped>
.header-container {
  width: 100%;
  height: 3.9rem;
  display: grid;
  grid-template-columns: 1fr 60% 5%;
}

.logo {
  align-self: center;
}

#light-or-dark {
  align-self: center;
  justify-self: center;
}

@media (max-width: 1000px) {
  .header-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 1rem;
  }

  #navigation-bar {
    display: none;
  }

  #light-or-dark {
    width: 10%;
  }
}
</style>
