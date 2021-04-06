<template>
  <div class="social-medias-container">
    <SocialMedia
      :icon="['fab', 'instagram']"
      url="https://www.instagram.com/igreja_batista_trindade/"
      class="social-media-item"
    />
    <SocialMedia
      :icon="['fab', 'facebook-square']"
      url="https://pt-br.facebook.com/ibatistatrindade/"
      class="social-media-item"
    />
    <SocialMedia
      :icon="['fab', 'youtube-square']"
      url="https://www.youtube.com/channel/UCftVBJhCf6Qt_ACrHOQipxg"
      class="social-media-item"
    />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style scoped>
.social-medias-container {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.social-media-item {
  width: 47px;
  height: 51px;
  margin-right: 30px;
}

.social-media-item:last-child {
  margin: 0;
}

@media (max-width: 1000px) {
  .social-medias-container {
    justify-content: center;
    align-items: center;
  }
}
</style>
