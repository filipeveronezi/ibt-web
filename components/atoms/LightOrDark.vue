<template>
  <div class="light-or-dark">
    <fa class="icon" icon="adjust" @click="toogleColorMode" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  methods: {
    toogleColorMode(): void {
      this.$colorMode.preference =
        this.$colorMode.preference === 'light' ? 'dark' : 'light'
    }
  }
})
</script>

<style scoped>
.light-or-dark {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.icon {
  cursor: pointer;
  max-width: 22px;
  max-height: 24px;
  width: 2.2rem;
  height: 2.4rem;
}
</style>
