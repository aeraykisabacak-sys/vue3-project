<script setup>
import { ref } from 'vue'

const sayac = ref(0)
const mesaj = ref('Merhaba Vue 3!')
</script>

<template>
  <main class="container">
    <h1>{{ mesaj }}</h1>
    <p>Basit bir Vue 3 tek sayfa uygulaması.</p>

    <div class="card">
      <p>Sayaç: <strong>{{ sayac }}</strong></p>
      <button @click="sayac++">Artır</button>
      <button @click="sayac = 0">Sıfırla</button>
    </div>
  </main>
</template>

<style scoped>
.container {
  max-width: 640px;
  margin: 4rem auto;
  padding: 2rem;
  font-family: system-ui, sans-serif;
  text-align: center;
}

h1 {
  color: #42b883;
}

.card {
  margin-top: 2rem;
  padding: 1.5rem;
  border: 1px solid #e5e7eb;
  border-radius: 8px;
}

button {
  margin: 0 0.5rem;
  padding: 0.5rem 1rem;
  background: #42b883;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 1rem;
}

button:hover {
  background: #369870;
}
</style>
