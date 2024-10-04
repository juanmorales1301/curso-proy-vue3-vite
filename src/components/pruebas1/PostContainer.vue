<template>
  <div class="post-container">
    <PostCard />
    <PostCard />
    <PostCard />
  </div>
</template>

<script lang="ts" setup>
import PostCard from '@/components/pruebas1/PostCard.vue'
</script>

<style scoped>
.post-container {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}
</style>
