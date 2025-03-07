<!-- components/Section.vue -->
<template>
    <section>
      <h2>{{ title }}</h2>
      <slot />
    </section>
  </template>
  
  <script>
  export default {
    props: {
      title: String,
    },
  };
  </script>
  
  <style scoped>
  section {
    margin-bottom: 2rem;
    padding: 1rem;
    background-color: #f5f5f5;
    border-radius: 10px;
  }
  
  h2 {
    color: #2c3e50;
  }
  </style>