<script setup lang="ts">
import ImageCarousel from "@/components/ui/ImageCarousel.vue";
const items = [
  {
    key: '1',
    src: new URL('@/assets/logos/vuejs.svg', import.meta.url).href,
    alt: "Vue.js"
  },
  {
    key: '2',
    src: new URL('@/assets/logos/css.svg', import.meta.url).href,
    alt: "Css"
  },
  {
    key: '3',
    src: new URL('@/assets/logos/csharp.svg', import.meta.url).href,
    alt: "Csharp"
  },
  {
    key: '4',
    src: new URL('@/assets/logos/dbs-redis.svg', import.meta.url).href,
    alt: "Redis"
  },
  {
    key: '5',
    src: new URL('@/assets/logos/html.svg', import.meta.url).href,
    alt: "HTML"
  },
  {
    key: '6',
    src: new URL('@/assets/logos/dotnet.svg', import.meta.url).href,
    alt: "DotNet"
  },
  {
    key: '7',
    src: new URL('@/assets/logos/mysql.svg', import.meta.url).href,
    alt: "MySQL"
  },
  {
    key: '8',
    src: new URL('@/assets/logos/php.svg', import.meta.url).href,
    alt: "PHP"
  },
  {
    key: '9',
    src: new URL('@/assets/logos/wordpress.svg', import.meta.url).href,
    alt: "Wordpress"
  }
];
const compositedItems = [...items, ...items];
</script>

<template>
  <section class="coreTechnologies">
    <div class="container-core-technologies-content">
      <h2>Core Technologies</h2>
      <ImageCarousel :items="compositedItems"/>
    </div>
  </section>
</template>

<style scoped>
h2 {
  font-family: var(--font-headline),serif;
  font-size: 4rem;
  font-weight: 500;
  text-align: center;
  margin-top: 2rem;
  color: var( --vt-c-white);
  line-height: 0;
}
.coreTechnologies{
  padding: 7.8rem 0;
}
</style>