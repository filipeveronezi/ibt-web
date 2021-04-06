<template>
  <div class="quick-access-container">
    <div class="item-container calendar">
      <img
        v-if="colorMode === 'light'"
        src="@/assets/img/calendar-light.svg"
        alt="Agenda"
      />
      <img
        v-if="colorMode === 'dark'"
        src="@/assets/img/calendar-dark.svg"
        alt="Agenda"
      />
      <p>Agenda</p>
    </div>
    <div class="item-container sermons">
      <p>Sermões</p>
      <img
        v-if="colorMode === 'light'"
        src="@/assets/img/sermons-light.svg"
        alt="Sermões"
      />
      <img
        v-if="colorMode === 'dark'"
        src="@/assets/img/sermons-dark.svg"
        alt="Sermões"
      />
    </div>
    <div class="item-container podcasts">
      <img
        v-if="colorMode === 'light'"
        src="@/assets/img/podcasts-light.svg"
        alt="Podcasts"
      />
      <img
        v-if="colorMode === 'dark'"
        src="@/assets/img/podcasts-dark.svg"
        alt="Podcasts"
      />
      <p>Podcasts</p>
    </div>
    <div class="item-container visit">
      <p>Visite-nos</p>
      <img
        v-if="colorMode === 'light'"
        src="@/assets/img/visit-light.svg"
        alt="Visite-nos"
      />
      <img
        v-if="colorMode === 'dark'"
        src="@/assets/img/visit-dark.svg"
        alt="Visite-nos"
      />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  computed: {
    colorMode(): string {
      return this.$colorMode.value
    }
  }
})
</script>

<style scoped>
.quick-access-container {
  width: 100%;
  max-height: 300px;
  max-width: 580px;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.item-container {
  position: absolute;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  transition: transform 0.3s;
}

.item-container img {
  cursor: pointer;
}

.item-container:hover {
  transform: scale(1.1);
}

.calendar {
  left: 0;
  top: 5px;
}

.sermons {
  left: 130px;
  bottom: 5px;
}

.podcasts {
  left: 260px;
  top: 5px;
}

.visit {
  left: 390px;
  bottom: 5px;
}

.calendar p,
.podcasts p {
  margin-top: 7px;
}

.sermons p,
.visit p {
  margin-bottom: 7px;
}

p {
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  font-size: 1.3rem;
  font-weight: 400;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

@media (max-width: 1000px) {
  .item-container img {
    width: 100px;
    height: 100px;
  }

  .calendar {
    left: 0;
    top: 5px;
  }

  .sermons {
    left: 67px;
    bottom: 5px;
  }

  .podcasts {
    left: 134px;
    top: 5px;
  }

  .visit {
    left: 201px;
    bottom: 5px;
  }

  .calendar p,
  .podcasts p {
    margin-top: 4px;
  }

  .sermons p,
  .visit p {
    margin-bottom: 4px;
  }

  p {
    font-size: 0.9rem;
  }
}
</style>
