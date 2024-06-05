<script setup lang="ts">
import Hero from "@/views/Home/Hero.vue";
import Services from "@/views/Home/Services.vue";
</script>

<template>
  <div class="home">
    <Hero/>
    <Services/>  
  </div>
</template>

<style scoped>
.home
{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
}
</style>