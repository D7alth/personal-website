<script setup lang="ts">
 import {FontAwesomeIcon} from "@fortawesome/vue-fontawesome";
 const props = defineProps<{
   brandingStyle: string;
   icon: [string, string]; 
   text: string;
 }>();
</script>

<template>
  <a :class="props.brandingStyle">
    <font-awesome-icon :icon="props.icon"></font-awesome-icon> {{props.text}}
  </a>
</template>

