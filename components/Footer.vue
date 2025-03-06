<!-- components/NavigationBar.vue -->
<template>
    <nav class="navigation-bar">
      <div class="logo">
        <img src="~/assets/logo.png" alt="Logo" />
      </div>
      <ul class="menu">
        <li v-for="item in menuItems" :key="item.name">
          <NuxtLink :to="item.path">{{ item.name }}</NuxtLink>
        </li>
      </ul>
    </nav>
  </template>
  
  <script>
  import menuItems from '~/assets/data/menu.js';
  
  export default {
    data() {
      return {
        menuItems
      };
    }
  };
  </script>
  
  <style scoped>
  .navigation-bar {
    position: sticky;
    top: 0;
    z-index: 1000;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #333;
    padding: 1rem;
  }
  .logo img {
    height: 50px;
  }
  .menu {
    list-style: none;
    display: flex;
    gap: 1rem;
  }
  .menu a {
    color: white;
    text-decoration: none;
  }
  @media (max-width: 768px) {
    .navigation-bar {
      flex-direction: column;
    }
    .menu {
      flex-direction: column;
      align-items: center;
    }
  }
  </style>