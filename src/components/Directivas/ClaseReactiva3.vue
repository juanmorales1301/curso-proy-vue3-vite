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

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'ClaseReactiva3',
  setup() {
    let c = ref('#fff')
    const handleClick = () => (c.value = 'red')

    return { c, handleClick }
  }
})
</script>

<style scoped></style>
