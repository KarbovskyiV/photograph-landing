<template>
  <div class="about-me-container">
    <BaseHeader name="About Me" />
    <section class="d-flex justify-content-between">
      <div class="image-container">
        <img class="about-me-img" src="../assets/about-me.png" alt="Image" />
      </div>
      <div class="text-container">
        <div class="about-me-text">
          <p class="description">
            I am Victoria, a sorceress of light and shadow, weaving dreams into reality through the
            lens of my enchanted camera. In a realm where imagination and reality intertwine, I
            capture moments that sparkle with magic and wonder.
          </p>
          <p class="description">
            Each click of my camera opens a portal to fantastical worlds, where every portrait tells
            a story and every scene becomes a legend.
          </p>
          <p class="description">Prepare to be enchanted, for your story awaits to be unveiled.</p>
        </div>
        <div class="image-container-second">
          <img
            class="half-open-red-peony-img"
            src="../assets/half-open-red-peony.png"
            alt="Half open red peony"
          />
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import BaseHeader from '@/components/Headers/BaseHeader.vue'
</script>

<style scoped>
.about-me-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
  margin-top: 120px;

  section {
    margin-top: 64px;

    .image-container {
      width: 455px;
      height: 479px;
      margin-right: 216px;

      .about-me-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }

    .text-container {
      width: 455px;
      height: 479px;
      text-align: left;
      position: relative;

      .about-me-text {
        width: 455px;
        height: 247px;

        .description {
          font-family: 'Montserrat';
          font-size: 16px;
          font-weight: 400;
          line-height: 24px;
          text-align: left;
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

        .half-open-red-peony-img {
          width: 100%;
          height: 100%;
          object-fit: cover;
        }
      }
    }
  }
}
</style>
