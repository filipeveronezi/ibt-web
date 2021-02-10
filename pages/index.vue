<template>
  <div class="container">
    <h1 class="title">Igreja Batista da Trindade</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  layout: 'default',
  data() {
    return {
      data: ''
    }
  }
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;300;400;500;700&family=Oxygen:wght@300;400;700&display=swap');

.container {
  margin: 0 auto;
  min-height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;
  background: #17252a;
}

.title {
  color: #fff;
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  letter-spacing: 0.2rem;
  text-transform: uppercase;
  cursor: default;
}
</style>
