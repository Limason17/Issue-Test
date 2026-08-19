<script setup>
import { ref } from 'vue'

const title = ref('Personenkarten')
const description = ref('Hier werden die Personenkarten der Teammitglieder angezeigt.')
</script>

<template>
  <div class="personenkarten-page">
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
  </div>
</template>

<style scoped>
.personenkarten-page {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  min-height: 80vh;
  text-align: center;
  padding: 20px;
}
</style>
