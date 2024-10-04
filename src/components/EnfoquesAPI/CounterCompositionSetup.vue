<template>
  <h3 id="titulo">{{ counter }}</h3>
  <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts" setup>
import { ref, type Ref } from 'vue'

let counter: Ref = ref(0)
const addCounter = () => {
  counter.value++
  console.log(counter)
}
</script>

<style>
#titulo {
  display: inline-block;
  color: darkblue;
}
</style>
