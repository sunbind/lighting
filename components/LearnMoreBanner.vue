<template>
    <div 
      v-if="isVisible" 
      class="fixed top-0 left-0 w-full bg-blue-600 text-white text-center p-3 transition-all duration-300"
      :class="{ '-translate-y-full': hideOnScroll }"
    >
      <p>
        새로운 기능이 추가되었습니다! <a href="/learn-more" class="underline">자세히 보기</a>
      </p>
      <button @click="closeBanner" class="absolute right-4 top-1/2 -translate-y-1/2 text-white">
        ✕
      </button>
    </div>
  </template>
  
  <script setup>
  import { ref, onMounted, onUnmounted } from "vue";
  
  const isVisible = ref(true); // X 버튼 클릭 시 false로 변경
  const hideOnScroll = ref(false);
  
  const handleScroll = () => {
    if (window.scrollY > 50) {
      hideOnScroll.value = true;
    } else {
      hideOnScroll.value = false;
    }
  };
  
  const closeBanner = () => {
    isVisible.value = false;
    localStorage.setItem("hideBanner", "true");
  };
  
  onMounted(() => {
    if (localStorage.getItem("hideBanner") === "true") {
      isVisible.value = false;
    }
    window.addEventListener("scroll", handleScroll);
  });
  
  onUnmounted(() => {
    window.removeEventListener("scroll", handleScroll);
  });
  </script>
  
  <style scoped>
  /* 스크롤 시 숨김 애니메이션 */
  .-translate-y-full {
    transform: translateY(-100%);
  }
  </style>
  