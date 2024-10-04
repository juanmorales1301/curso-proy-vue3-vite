<template>
  <p
    v-bind:style="{
      backgroundColor: 'rgb(220,220,220)',
      color: c
    }"
  >
    El mensaje se ha enviado satisfactoriamente
  </p>

  <!--<button v-on:click="handleClick()">Cambiar color</button> funciona igual-->
  <button @click="handleClick()">Cambiar color</button>
</template>

<script setup lang="ts">
import { ref, type Ref } from 'vue'

let c: Ref<string> = ref('#fff')
const handleClick = () => (c.value = 'red')
</script>

<style scoped></style>
