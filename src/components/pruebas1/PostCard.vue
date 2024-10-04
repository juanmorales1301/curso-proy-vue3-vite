<template>
  <div class="post-card">
    <h3>Titulo</h3>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Modi aliquam, reiciendis adipisci,
      fuga accusamus nam odio eos enim a consequuntur vitae labore quas voluptatibus animi? Expedita
      ut quas ab. Qui?
    </p>
    <PostButton />
  </div>
</template>

<script lang="ts" setup>
import PostButton from '@/components/pruebas1/PostButton.vue'
</script>

<style scoped>
.post-card {
  border-radius: 15px;
  padding: 10px;
  margin: 0px;
  border: 1px solid #ccc;
}
</style>
