<script>

import { defineComponent } from 'vue'
import VHeader from '@/components/Header.vue'
import Watch from '@/components/Watch.vue'
import Date from '@/components/Date.vue'

export default defineComponent({
  components: {
    VHeader,
    Date,
    Watch
  }
})
</script>

<template>
  <VHeader></VHeader>
  <main class="app-container">
    <div class="wrapper">
      <Date></Date>
      <Watch></Watch>
    </div>
  </main>
</template>

<style>
.app-container {
  width: 100%;
}

.wrapper {
  margin: 0 auto;
}
</style>
