<script setup lang="ts">
const props = defineProps<{
  items: {
    src: string;
    alt: string;
  }[];
}>();
</script>

<template>
  <div class="carousel">
    <div class="carousel-track">
      <div class="carousel-item" v-for="item in props.items">
        <img :src="item.src" :alt="item.alt">
      </div>
    </div>
  </div>
</template>

<style scoped>
@keyframes scroll {
  from {
    transform: translateX(calc(42% + 10px));
  }
  to {
    transform: translateX(calc(
        -100px * 6
    ));
  }
}
.carousel {
  height: 100px;
  position: relative;
  width: 100%;
  background: rgba(255, 255, 255, 0.6);
  padding: 1rem;
  overflow: hidden;
}
.carousel::before, .carousel::after {
  background: radial-gradient(circle, rgba(255,255,255,1) 0%, rgba(255,255,255,0) 0%, rgba(255,255,255,1) 30%);
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
  width: 140%;
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
