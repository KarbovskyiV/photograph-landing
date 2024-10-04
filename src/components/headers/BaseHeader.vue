<template>
  <div class="h-2-container">
    <DecorLeft />
    <span>{{ name }}</span>
    <DecorRight />
  </div>
</template>

<script setup>
import DecorLeft from '@/components/icons/DecorLeft.vue';
import DecorRight from '@/components/icons/DecorRight.vue';

defineProps({
  name: String,
});
</script>

<style scoped>
.h-2-container {
  display: flex;
  justify-content: center;
  align-items: center;
}

span {
  font-size: 40px;
  font-weight: 600;
  line-height: 60px;
}
</style>
