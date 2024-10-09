<template>
  <div
    @mouseover="hovering = true"
    @mouseleave="hovering = false"
    class="button"
    :style="{ marginTop: `${marginTop}px`, marginLeft: `${marginLeft}px` }"
  >
    <Subtract v-if="hovering" />
    <span @click="scrollToPortfolio" class="text" :style="{ padding: hovering ? '0 6px' : '0' }">
      {{ name }}
    </span>
    <Subtract v-if="hovering" />
  </div>
</template>

<script setup>
import Subtract from '@/components/icons/Subtract.vue';
import { ref } from 'vue';

defineProps({
  name: {
    type: String,
    required: true,
  },
  marginTop: {
    type: [String, Number],
    default: 44,
  },
  marginLeft: {
    type: [String, Number],
    default: 393,
  },
});

const hovering = ref(false);

const scrollToPortfolio = () => {
  const portfolioSection = document.getElementById('portfolio-section');
  if (portfolioSection) {
    portfolioSection.scrollIntoView({ behavior: 'smooth' });
  }
};
</script>

<style scoped>
.button {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 256px;
  height: 56px;
  border: 1px solid #e5e1d2;
  cursor: pointer;

  .text {
    font-family: 'Montserrat';
  }
}
</style>
