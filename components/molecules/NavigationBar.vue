<template>
  <nav class="nav-bar-container">
    <div class="overlay"></div>
    <ul class="nav-bar-list">
      <NuxtLink to="/" :class="`nav-bar-item ${checkActive('/')}`"
        >Início</NuxtLink
      >
      <NuxtLink
        to="quem-somos"
        :class="`nav-bar-item ${checkActive('/quem-somos')}`"
        >Quem somos</NuxtLink
      >
      <NuxtLink
        to="conteudo"
        :class="`nav-bar-item ${checkActive('/conteudo')}`"
        >Conteúdo</NuxtLink
      >
      <NuxtLink to="contato" :class="`nav-bar-item ${checkActive('/contato')}`"
        >Contato</NuxtLink
      >
      <a class="blog">Blog</a>
    </ul>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  computed: {
    currentPath(): String {
      return this.$route.fullPath
    }
  },
  methods: {
    checkActive(path: String) {
      if (path === this.currentPath) {
        return 'is-active'
      } else {
        return ''
      }
    }
  }
})
</script>

<style scoped>
.nav-bar-container {
  width: 100%;
  height: 100%;
  display: grid;
  place-items: center;
}

.nav-bar-list {
  width: 100%;
  list-style-type: none;

  display: flex;
  flex-direction: row;

  align-items: center;
  justify-content: space-evenly;
}

.nav-bar-item {
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
  letter-spacing: 0.15rem;
  text-indent: 0.15rem;
  text-transform: uppercase;
  text-decoration: none;
  color: var(--color);
  cursor: pointer;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.nav-bar-item:after {
  content: '';
  width: 100%;
  height: 4px;
  display: block;
  position: absolute;
  top: 20px;
  visibility: hidden;
  transition: 0.3s;
}

.is-active:after {
  content: '';
  width: 100%;
  height: 4px;
  display: block;
  position: absolute;
  background-color: var(--color-secondary);
  visibility: visible;
  top: 20px;
}

.nav-bar-item:hover::after {
  background-color: var(--color-secondary);
  opacity: 0.3;
  visibility: visible;
}

.blog {
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
  letter-spacing: 0.15rem;
  text-transform: uppercase;
  display: grid;
  place-items: center;
  width: 96px;
  height: 28px;
  border-radius: 8px;
  background: var(--button);
  color: var(--white);
  cursor: pointer;
  border: none;
  text-decoration: none;
  transition: background-color 0.3s;
}

.blog:hover {
  background: var(--button-hover);
}
</style>
