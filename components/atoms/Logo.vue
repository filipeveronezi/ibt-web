<template>
  <div :style="`width: ${width}; height: ${height}`">
    <img
      v-if="colorMode === 'light'"
      src="@/assets/img/logo-light.svg"
      alt="Logotipo de Igreja Batista da Trindade"
      class="logo"
    />
    <img
      v-if="colorMode === 'dark'"
      src="@/assets/img/logo-dark.svg"
      alt="Logotipo de Igreja Batista da Trindade"
      class="logo"
    />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    width: {
      type: String,
      default: '47px'
    },
    height: {
      type: String,
      default: '39px'
    }
  },
  computed: {
    colorMode(): string {
      return this.$colorMode.value
    }
  }
})
</script>

<style scoped>
.logo {
  width: 100%;
  height: 100%;
}
</style>
