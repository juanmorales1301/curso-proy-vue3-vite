<template>
  <h1 v-if="age < 18">Eres menor de edad</h1>
  <h1 v-else-if="age >= 18">Eres mayor de edad</h1>
</template>

<script setup lang="ts">
import { ref } from 'vue'

let age = ref(15)
let interval = setInterval(() => {
  age.value++
  console.log(age.value)
}, 1000)

setTimeout(() => {
  clearInterval(interval)
}, 10000)
</script>

<style scoped></style>
