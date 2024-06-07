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
    <div class="carousel-track">
      <div class="carousel-item" v-for="item in props.items" :key="item.key">
        <img :src="item.src" :alt="item.alt">
      </div>
    </div>
  </div>
</template>

<style scoped>
@keyframes scroll {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(calc(
        -100px * 10));
  }
}
.carousel {
  height: 100px;
  position: relative;
  width: 100%;
  background: white;
  padding: 1rem;
}
.carousel::before, .carousel::after {
  background: radial-gradient(circle, rgba(255,255,255,1) 0%, rgba(255,255,255,0) 0%, rgba(255,255,255,1) 35%);
  content: "";
  height: 100px;
  position: absolute;
  width: 100%;
}
.carousel::after {
  right: 0;
  top: 0;
  transform: rotateZ(180deg);
}
.carousel::before {
  left: 0;
  top: 0;
}
.carousel-track {
  overflow: hidden;
  display: flex;
  animation: scroll 20s linear infinite;
  width: calc(100px * 30);
}
.carousel-item {
  height: 60px;
  flex: 0 0 auto;
  width: 200px;
}
img {
  height: 60px;
 
  object-fit: cover;
  margin: 0 1rem;
}
</style>
