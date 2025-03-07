<!-- layouts/default.vue -->
<template>
    <div>
      <NavigationBar />
      <Nuxt />
    </div>
  </template>
  
  <script>
  import LearnMoreBanner from "~/components/LearnMoreBanner.vue";
  import NavigationBar from '~/components/NavigationBar.vue';
  import Footer from '~/components/Footer.vue';
  
  export default {
    components: {
      LearnMoreBanner,
      NavigationBar,
      Footer
    }
  };
  </script>