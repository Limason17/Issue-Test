<script setup>
import { ref } from 'vue'
import Navigation from './components/Navigation.vue'
import Startpage from './components/Startpage.vue'
import Personenkarte from './components/Personenkarte.vue'

const currentTab = ref('start')
</script>

<template>
  <div class="app-layout">
    <Navigation :active-tab="currentTab" @update:active-tab="currentTab = $event" />
    <main class="main-content">
      <Startpage v-if="currentTab === 'start'" />
      <Personenkarte v-else-if="currentTab === 'team'" />
    </main>
  </div>
</template>

<style scoped>
.app-layout {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  width: 100%;
}

.main-content {
  flex: 1;
  width: 100%;
}
</style>
