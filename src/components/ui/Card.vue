<script setup lang="ts">
  const props = defineProps<{
    title: string;
  }>();
</script>

<template>
  <div class="card">
    <h3 class="card-title">{{props.title}}</h3>
    <slot></slot>
  </div>
</template>

<style scoped>
  .card
  {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: start;
    width: 25%;
    padding: 1rem;
    margin: 0.3rem;
    border: 1px solid #ccc;
    border-radius: 5px;
    text-align: left;
    
  }
  .card-title
  {
    font-size: 2rem;
    margin-bottom: 1rem;
  }
</style>