<template>
  <p
    v-bind:class="{
      danger: hasError
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

<style scoped>
.danger {
  color: red;
}
</style>
