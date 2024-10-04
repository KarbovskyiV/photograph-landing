<template>
  <div class="portfolio-container">
    <BaseHeader name="Portfolio" />
    <Portraits />
    <PersonalPhotoShoot />
  </div>
</template>

<script setup>
import BaseHeader from '@/components/headers/BaseHeader.vue';
import Portraits from '@/components/portfolio/FirstSection.vue';
import PersonalPhotoShoot from '@/components/portfolio/SecondSection.vue'
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
