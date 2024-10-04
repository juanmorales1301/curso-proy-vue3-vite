<template>
  <p
    v-bind:style="{
      backgroundColor: hasError ? 'transparent' : '#ccc',
      color: hasError ? 'red' : '#fff'
    }"
  >
    El mensaje se ha enviado satisfactoriamente
  </p>
</template>

<script setup lang="ts">
import { ref, type Ref } from 'vue'

let hasError: Ref = ref(false)

setTimeout(() => {
  hasError.value = true
}, 2000)
</script>

<style scoped></style>
