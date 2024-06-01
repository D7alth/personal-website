<script setup lang="ts">
 import {FontAwesomeIcon} from "@fortawesome/vue-fontawesome";
 const props = defineProps<{
   brandingStyle: string;
   icon: [string, string]; 
   text: string;
   link: string;
 }>();
</script>

<template>
  <a :href="props.link" :class="props.brandingStyle">
    <font-awesome-icon :icon="props.icon"></font-awesome-icon> {{props.text}}
  </a>
</template>

