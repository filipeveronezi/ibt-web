<template>
  <div class="social-medias-container">
    <SocialMedia
      :icon="['fab', 'instagram']"
      url="https://www.instagram.com/igreja_batista_trindade/"
    />
    <SocialMedia
      :icon="['fab', 'facebook-square']"
      url="https://pt-br.facebook.com/ibatistatrindade/"
    />
    <SocialMedia
      :icon="['fab', 'youtube-square']"
      url="https://www.youtube.com/channel/UCftVBJhCf6Qt_ACrHOQipxg"
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
  justify-content: center;
}
</style>
