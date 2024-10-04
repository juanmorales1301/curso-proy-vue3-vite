<template>
  <h3 id="titulo">{{ counter }}</h3>
  <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts">
import { defineComponent, ref, type Ref } from 'vue'

export default defineComponent({
  name: 'CounterComposition',
  setup() {
    let counter: Ref = ref(0)
    const addCounter = () => {
      counter.value++
      console.log(counter)
    }

    return { counter, addCounter }
  }
})
</script>

<style>
#titulo {
  display: inline-block;
  color: darkblue;
}
</style>
