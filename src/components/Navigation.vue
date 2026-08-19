<script setup>
defineProps({
  activeTab: {
    type: String,
    default: 'start'
  }
})

const emit = defineEmits(['update:activeTab'])

function selectTab(tab) {
  emit('update:activeTab', tab)
}
</script>

<template>
  <header class="navbar">
    <div class="navbar-container">
      <div class="navbar-brand">
        <h2>Projekt-Team</h2>
      </div>
      <nav class="navbar-nav">
        <ul>
          <li>
            <button
              :class="{ active: activeTab === 'start' }"
              @click="selectTab('start')"
            >
              Startseite
            </button>
          </li>
          <li>
            <button
              :class="{ active: activeTab === 'team' }"
              @click="selectTab('team')"
            >
              Personenkarten
            </button>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style scoped>
.navbar {
  width: 100%;
  border-bottom: 1px solid #e2e8f0;
  background-color: #ffffff;
}

.navbar-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem 1.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.navbar-brand h2 {
  margin: 0;
  font-size: 1.25rem;
}

.navbar-nav ul {
  display: flex;
  list-style: none;
  gap: 1rem;
  margin: 0;
  padding: 0;
}

.navbar-nav button {
  background: none;
  border: 1px solid transparent;
  padding: 0.5rem 1rem;
  font-size: 1rem;
  cursor: pointer;
  border-radius: 4px;
}

.navbar-nav button.active {
  font-weight: bold;
  border-color: #213547;
}
</style>
