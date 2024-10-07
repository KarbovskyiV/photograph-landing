<template>
  <div class="services-container">
    <BaseHeader name="Reviews" />

    <section>
      <div class="reviews-text">
        <p class="title">Emily & James T</p>
        <span class="description">
          Working with Victoria was like stepping into a fairytale. The attention to detail and the ability to capture
          the essence of our love was truly remarkable. The portraits are more than just pictures; they are magical
          memories we’ll cherish forever.
        </span>
      </div>
      <div class="reviews-text">
        <p class="title">LILY S</p>
        <span class="description">
          From start to finish, Victoria made us feel like stars in our own fantasy world. The creative vision and the
          way she brought our ideas to life was incredible. The photo shoot was not only fun but also resulted in
          stunning, imaginative portraits we absolutely adore. We couldn’t be happier with the results! Thank you so
          much!
        </span>
      </div>
      <div class="reviews-text">
        <p class="title">Sarah & David</p>
        <span class="description">
          The photos are beautiful and tell our story asdsaddassad made us feel comfortable and relaxed, al
          asdsadasdasdads selves to shine through.
        </span>
      </div>
    </section>

    <div class="carousel-section">
      <i class="bi bi-arrow-left me-3 opacity-50"></i>
      <i class="bi bi-arrow-right"></i>
    </div>
  </div>
</template>

<script setup>
import BaseHeader from '@/components/headers/BaseHeader.vue';
</script>

<style scoped>
.services-container {
  display: flex;
  align-items: center;
  flex-direction: column;

  section {
    display: flex;
    margin-top: 64px;
    max-width: 1130px;
    overflow: hidden;

    .reviews-text {
      width: 455px;
      flex-shrink: 0;
      margin-right: 24px;

      .title {
        font-family: 'Montserrat';
        font-size: 20px;
        line-height: 20px;
      }

      .description {
        font-family: 'Montserrat';
      }
    }
  }

  .carousel-section {
    display: flex;
    align-items: flex-start;
    width: 1130px;
    margin-top: 44px;

    i {
      font-size: 24px;
      cursor: pointer;
    }
  }
}
</style>
