<template>
  <div class="index">
    <div class="left-side">
      <h1 class="title">Igreja Batista da Trindade</h1>
      <SocialMedias class="social-medias" />
    </div>
    <div class="right-side">
      <QuickAccess />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style scoped>
.index {
  width: 100%;
  height: 80%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.left-side,
.right-side {
  width: 50%;
}

.title {
  font-family: 'Montserrat', sans-serif;
  text-transform: uppercase;
  font-size: 4rem;
  font-weight: 700;
  letter-spacing: 9px;
  line-height: 90px;
  width: 100%;
  margin: 0;
  transition: letter-spacing 0.3s;
  transition-timing-function: ease;
}

.social-medias {
  margin-top: 23px;
  width: 200px;
  height: 50px;
}
</style>
