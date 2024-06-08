<script setup lang="ts">
import ImageCarousel from "@/components/ui/ImageCarousel.vue";

const items = [
  {
   src: new URL('@/assets/logos/php.svg', import.meta.url).href,
    alt: "PHP"
  },
  {
    src: new URL('@/assets/logos/mysql.svg', import.meta.url).href,
    alt: "MySQL"
  },
  {
    src: new URL('@/assets/logos/vuejs.svg', import.meta.url).href,
    alt: "Vue.js"
  },
  {
    src: new URL('@/assets/logos/dotnet.svg', import.meta.url).href,
    alt: "Dotnet"
  },
  {
    src: new URL('@/assets/logos/nodejs.svg', import.meta.url).href,
    alt: "Nodejs"
  },
  {
    src: new URL('@/assets/logos/postgresql.svg', import.meta.url).href,
    alt: "PostgreSQL"
  },
  {
    src: new URL('@/assets/logos/vc-git.svg', import.meta.url).href,
    alt: "Git"
  }
];
const duplicatedArray = items.concat(items);
</script>

<template>
  <section class="technologies">
    <ImageCarousel :items="duplicatedArray"/>
  </section>
</template>
  
<style scoped>

</style>