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
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'ClaseReactiva2',
  data() {
    return {
      c: '#fff'
    }
  },
  methods: {
    handleClick() {
      this.c = 'red'
    }
  }
})
</script>

<style scoped></style>
