<template>
    <div class="service-card">
      <h3>{{ title }}</h3>
      <p>{{ description }}</p>
    </div>
  </template>
  
  <script setup>
  const props = defineProps({
    title: String,
    description: String,
  })
  </script>
  
  <style scoped>
  .service-card {
    border: 1px solid #ccc;
    padding: 1rem;
    margin: 1rem 0;
  }
  </style>