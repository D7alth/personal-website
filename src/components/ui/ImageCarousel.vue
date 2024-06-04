<script setup lang="ts">
const props = defineProps<{
  items: {
    key: string;
    src: string;
    alt: string;
  }[];
}>();
</script>

<template>
  <div class="carousel">
      <div class="carousel-item" v-for="item in props.items" :key="item.key">
        <img :src="item.src" :alt="item.alt">
      </div>
  </div>
</template>

<style scoped>

@keyframes slide {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-100%);
  }
}
.carousel {
  scroll-snap-type: x mandatory;
  -webkit-overflow-scrolling: touch;
  scroll-behavior: smooth;
  overflow: hidden;
  white-space: nowrap;
  padding: 4rem 0;
  max-width: 600px;
}
.carousel-item {
  display: inline-block;
  animation: 3s slide infinite;
}
img {
  height: 4rem;
  filter: invert(1);
  margin: 0 3rem;
}
</style>