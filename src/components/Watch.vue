<script setup>
import { onMounted, reactive, ref, watch } from 'vue'

const date = new Date();
const currentTime = ref('');

onMounted(() => {
  const intervalId = setInterval(() => {
    const now = new Date();
    const hours = now.getHours().toString().padStart(2, '0');
    const minutes = now.getMinutes().toString().padStart(2, '0');
    const seconds = now.getSeconds().toString().padStart(2, '0');
    currentTime.value = `${hours}:${minutes}:${seconds}`;
  }, 1000);

  // 컴포넌트가 언마운트될 때 인터벌 해제
  onUnmounted(() => clearInterval(intervalId));
})
</script>

<template>
  <h1>{{ currentTime }}</h1>
</template>

<style>

</style>
