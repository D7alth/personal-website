<script setup lang="ts">
import Hero from "@/views/Home/Hero.vue";
import CoreTechnologies from "@/views/Home/CoreTechnologies.vue";
</script>

<template>
  <div class="home">
    <Hero/>
    <CoreTechnologies/>  
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