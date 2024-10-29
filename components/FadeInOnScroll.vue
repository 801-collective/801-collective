<template>
    <div
      :class="{
        'opacity-0 translate-y-4': !isVisible,
        'opacity-100 translate-y-0': isVisible,
        'transition-opacity transform duration-700 ease-out': true,
      }"
    >
      <slot />
    </div>
  </template>

  <script setup>
  import { ref, onMounted, onUnmounted } from 'vue';

  const isVisible = ref(false);
  const elementRef = ref(null);

  onMounted(() => {
    const observer = new IntersectionObserver(
      ([entry]) => {
        if (entry.isIntersecting) {
          isVisible.value = true;
          observer.unobserve(entry.target); // Only trigger once
        }
      },
      {
        threshold: 0.1, // Adjust visibility threshold (0.1 = 10% visible)
      }
    );

    if (elementRef.value) {
      observer.observe(elementRef.value);
    }

    onUnmounted(() => {
      observer.disconnect();
    });
  });
  </script>

  <style scoped>
  /* Additional styles can be defined here if needed */
  </style>
