<script setup>
import { useBreakpoints } from '@vueuse/core';
const breakpoints = useBreakpoints({ lg: 1024 });
console.log(breakpoints);
</script>

<template>
  <h1>Hello VueUse!</h1>
  <a
    href="https://vueuse.org/"
    target="_blank"
    v-if="toValue(breakpoints.greaterOrEqual('lg'))"
    >Documentation</a
  >
</template>

<style></style>
