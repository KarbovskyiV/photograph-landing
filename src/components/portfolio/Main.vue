<template>
  <div class="portfolio-container">
    <BaseHeader name="Portfolio" />
    <Portraits />
  </div>
</template>

<script setup>
import BaseHeader from '@/components/headers/BaseHeader.vue';
import Portraits from '@/components/portfolio/Portraits.vue';
</script>

<style scoped>
.portfolio-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
  margin-top: 120px;
}
</style>
