<template>
  <div class="portfolio-container">
    <BaseHeader name="Portfolio" />
    <FirstSection />
    <SecondSection />
    <ThirdSection />
  </div>
</template>

<script setup>
import BaseHeader from '@/components/headers/BaseHeader.vue';
import FirstSection from '@/components/portfolio/FirstSection.vue';
import SecondSection from '@/components/portfolio/SecondSection.vue';
import ThirdSection from '@/components/portfolio/ThirdSection.vue';
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
