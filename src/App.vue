<script setup>
  import { ref } from 'vue'

  const Contador = ref(0)

  function incrementar() {
    Contador.value++
  }
  function decrementar() {
    Contador.value--
  }
</script>

<template>
    <h1>Contador do Sombrio</h1>
    <p>Valor do Contador: {{ Contador }}</p>
    <button v-on:click="incrementar">+</button>
    <button @click="decrementar">-</button>
</template>

<style scoped>



</style>
