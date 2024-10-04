<template>
  <div>
    <section>
      <div class="d-flex justify-content-between">
        <span class="body-head">LOVE PHOTO SHOOT</span>
        <span class="body-right">Gallery of memories that shines as brightly as your hearts</span>
      </div>

      <div class="grid-container">
        <div class="left-image-container">
          <img class="image-cover" src="../../assets/portfolio/thirdSection/left-img.png" alt="Left image" />
        </div>

        <div class="top-right-image-container">
          <img class="image-cover" src="../../assets/portfolio/thirdSection/right-top-img.png" alt="Top right image" />
        </div>

        <div class="bottom-right-image-container">
          <img
            class="image-cover"
            src="../../assets/portfolio/thirdSection/right-bottom-img.png"
            alt="Bottom right image"
          />
        </div>
      </div>
    </section>
  </div>
</template>

<script setup></script>

<style scoped>
@import '@/assets/global.css';

section {
  margin-top: 48px;

  .body-head {
    font-family: 'Montserrat';
    font-size: 20px;
    line-height: 20px;
  }

  .body-right {
    font-family: 'Montserrat';
  }

  .grid-container {
    display: grid;
    gap: 24px;
    margin-top: 48px;

    .left-image-container {
      grid-row: 1 / 3;
      width: 456px;
    }

    .top-right-image-container {
      width: 360px;
      height: 413px;
      justify-self: end;
    }

    .bottom-right-image-container {
      grid-row: 2;
      display: flex;
      gap: 25px;
      width: 648px;
      height: 470px;
    }
  }
}
</style>
