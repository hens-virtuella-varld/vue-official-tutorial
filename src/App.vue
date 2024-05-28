<script setup>
import { ref, reactive } from 'vue';

const message = ref('Hello Universe!');

const laptop = reactive({
  brand: 'Apple',
  model: 'MacBook Air',
  chip: 'M3',
  year: 2024,
  size: 13,
  color: 'Space Gray',
  ram: '8GB',
  storage: '256GB',
});
</script>

<template>
  <h1>{{ message }}</h1>
  <p>{{ `${laptop.model} ${laptop.chip} will be an old model in ${laptop.year + 1}`}}</p>
</template>
<style scoped></style>
