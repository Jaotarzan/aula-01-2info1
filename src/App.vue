<script setup>
import { ref } from 'vue'

const contador = ref(0)

function decrementar() {
  if (contador.value > 0) contador.value--;
}
</script>

<template>
  <button @click="contador++">+</button>
  <button @click="decrementar">-</button>
  <button @click="contador = 0">0</button>
  <p>valor do contador: {{ contador }}</p>
</template>

<style scoped>
button {
  color: blueviolet;
  font-weight: bold;
  background-color: black;
  border: none;
}
</style>
