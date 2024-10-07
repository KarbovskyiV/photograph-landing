<template>
  <div class="about-me-container">
    <BaseHeader name="About Me" />

    <section class="d-flex">
      <div class="image-container">
        <img class="image-cover" src="../../assets/aboutMe/about-me.png" alt="Image" />
      </div>
      <div class="text-container">
        <div class="about-me-text">
          <p class="description">
            I am Victoria, a sorceress of light and shadow, weaving dreams into reality through the lens of my enchanted
            camera. In a realm where imagination and reality intertwine, I capture moments that sparkle with magic and
            wonder.
          </p>
          <p class="description">
            Each click of my camera opens a portal to fantastical worlds, where every portrait tells a story and every
            scene becomes a legend.
          </p>
          <p class="description">Prepare to be enchanted, for your story awaits to be unveiled.</p>
        </div>
        <div class="image-container-second">
          <img class="image-cover" src="../../assets/aboutMe/half-open-red-peony.png" alt="Half open red peony" />
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import BaseHeader from '@/components/headers/BaseHeader.vue';
</script>

<style scoped>
@import '@/assets/global.css';

.about-me-container {
  display: flex;
  align-items: center;
  flex-direction: column;
  margin-top: 120px;

  section {
    margin-top: 64px;

    .image-container {
      width: 455px;
      height: 479px;
      margin-right: 216px;
    }

    .text-container {
      position: relative;

      .about-me-text {
        width: 455px;

        .description {
          font-family: 'Montserrat';
          margin: 0 0 10px;
        }
      }

      .image-container-second {
        width: 187px;
        height: 161px;
        rotate: -30deg;
        position: absolute;
        bottom: 0;
        right: 0;
      }
    }
  }
}
</style>
