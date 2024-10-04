<template>
  <h3 id="titulo">{{ counter }}</h3>
  <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'CounterOption',
  data() {
    return { counter: 0 }
  },
  methods: {
    addCounter() {
      this.counter++
    }
  }
})
</script>

<style>
#titulo {
  display: inline-block;
  color: teal;
}
</style>
