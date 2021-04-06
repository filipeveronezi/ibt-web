<template>
  <div class="container">
    <slot />
  </div>
</template>

<style scoped>
.container {
  margin: 30px auto 0 auto;
  max-width: 1189px;
  width: 100%;
  height: 100%;
}

@media (max-width: 1000px) {
  .container {
    margin: 10px auto 0 auto;
  }
}
</style>
