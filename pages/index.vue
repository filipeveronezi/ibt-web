<template>
  <div class="index">
    <div class="left-side">
      <h1 class="title">Igreja Batista da Trindade</h1>
      <div class="social-medias-box">
        <SocialMedias class="social-medias" />
      </div>
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

.social-medias-box {
  width: 100%;
  height: 50px;
  margin-top: 23px;
}

@media (max-width: 1000px) {
  .index {
    flex-direction: column;
    justify-content: flex-start;
  }

  .left-side {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    width: 80%;
    height: 50%;
  }

  .right-side {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 300px;
    height: 30vh;
  }

  .title {
    text-align: center;
    font-size: 2rem;
    justify-self: flex-start;
    line-height: 60px;
  }
}

@media (max-height: 550px) {
  .right-side {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 300px;
    height: 60vh;
  }
}
</style>
