<template>
    <div>
      <h1>블로그</h1>
      <ul>
        <li v-for="post in posts" :key="post.id">
          <NuxtLink :to="`/blog/${post.id}`">{{ post.title }}</NuxtLink>
        </li>
      </ul>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  const posts = ref([
    { id: 1, title: 'Nuxt 3 배우기' },
    { id: 2, title: '웹 개발 팁과 트릭' },
  ])
  </script>