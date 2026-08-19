<script setup>
import { ref } from 'vue'

const title = ref('Willkommen zu unserem Projekt')
const description = ref('Dies ist die Startseite unseres GitHub-Projekts.')
</script>

<template>
  <div class="startpage">
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
  </div>
</template>

<style scoped>
.startpage {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  min-height: 80vh;
  text-align: center;
  padding: 40px 20px;
}

.startpage h1 {
  font-size: 2.5rem;
  margin-bottom: 16px;
}

.startpage p {
  font-size: 1.1rem;
  color: #64748b;
}
</style>
