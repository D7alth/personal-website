<script setup lang="ts">
  import CircleType from 'circletype' ;
  import {onMounted} from "vue";
  onMounted(() => {
    new CircleType(document.querySelector('.circular-animated-text > p')).radius(65);
  });
</script>

<template>
  <div class="circular-animated-text">
    <slot></slot>  
  </div>
</template>

<style scoped>
.circular-animated-text
{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 90px;
  height: 90px;
  margin: 10% auto -10%;
  animation: rotate 16s linear infinite;
  border: var(--vt-c-white) 1px solid;
  border-radius: 100%;
}
@keyframes rotate {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
</style>