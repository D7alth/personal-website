<script setup lang="ts">
import ImageCarousel from "@/components/ui/ImageCarousel.vue";

const items = [
  {
    key: "1",
    src: new URL('@/assets/logos/php.svg', import.meta.url).href,
    alt: "PHP"
  },
  {
    key: "2",
    src: new URL('@/assets/logos/mysql.svg', import.meta.url).href,
    alt: "MySQL"
  },
  {
    key: "3",
    src: new URL('@/assets/logos/vuejs.svg', import.meta.url).href,
    alt: "Vue.js"
  },
  {
    key: "4",
    src: new URL('@/assets/logos/dotnet.svg', import.meta.url).href,
    alt: "Dotnet"
  },
  {
    key: "5",
    src: new URL('@/assets/logos/wordpress.svg', import.meta.url).href,
    alt: "WordPress"
  },
  {
    key: "6",
    src: new URL('@/assets/logos/html.svg', import.meta.url).href,
    alt: "HTML"
  },
  {
    key: "7",
    src: new URL('@/assets/logos/css.svg', import.meta.url).href,
    alt: "CSS"
  },
  {
    key: "8",
    src: new URL('@/assets/logos/nodejs.svg', import.meta.url).href,
    alt: "Nodejs"
  },
  {
    key: "10",
    src: new URL('@/assets/logos/postgresql.svg', import.meta.url).href,
    alt: "PostgreSQL"
  },
  {
    key: "11",
    src: new URL('@/assets/logos/vc-git.svg', import.meta.url).href,
    alt: "Git"
  }
];
const duplicatedArray = [...items, ...items];
</script>

<template>
  <section class="technologies">
    <ImageCarousel :items="duplicatedArray"/>
  </section>
</template>
  
<style scoped>

</style>