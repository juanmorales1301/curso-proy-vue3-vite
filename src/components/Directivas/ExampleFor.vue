<template>
  <div>
    <ul>
      <li v-for="(country, index) in countries" v-bind:key="index">{{ country }}</li>
    </ul>
  </div>
  <hr />

  <div class="hr">
    <ul>
      <li v-for="country in countries" v-bind:key="country">{{ country }}</li>
    </ul>
  </div>
</template>

<script setup lang="ts">
import { ref, type Ref } from 'vue'

let countries: Ref<Array<string>> = ref(['España', 'Colombia', 'France'])
</script>

<style scoped></style>
