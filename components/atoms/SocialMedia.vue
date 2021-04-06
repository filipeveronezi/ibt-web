<template>
  <div class="social-media-container">
    <a :href="url" target="_blank" rel="noreferrer noopener">
      <fa class="icon" :icon="icon" />
    </a>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    url: {
      type: String,
      default: ''
    },
    icon: {
      type: Array,
      default: null
    }
  }
})
</script>

<style scoped>
.social-media-container {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

a {
  text-decoration: none;
  transition: transform 0.3s;
}

a:hover {
  transform: scale(1.1);
}

a,
.icon {
  width: 100%;
  height: 100%;
}

.icon {
  color: var(--color);
}
</style>
