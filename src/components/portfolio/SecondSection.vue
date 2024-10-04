<template>
  <div>
    <section>
      <div class="d-flex justify-content-between">
        <span class="body-head">PERSONAL PHOTO SHOOT</span>
        <span class="body-right">Dare to dream, and let’s create something truly magical</span>
      </div>

      <div class="grid-container">
        <div class="left-top-image-container">
          <img
            class="left-top-img"
            src="../../assets/portfolio/secondSection/left-top-img.png"
            alt="left top image"
          />
        </div>

        <div class="left-bottom-image-container">
          <img
            class="left-bottom-img"
            src="../../assets/portfolio/secondSection/left-bottom-img.png"
            alt="Left bottom image"
          />
          <div class="left-bottom-text">
            From the initial spark of inspiration to the final, stunning image, I will guide you
            through a tailored experience designed to reflect your individuality and style.
          </div>
        </div>

        <div class="right-image-container">
          <img
            class="right-img"
            src="../../assets/portfolio/secondSection/right-img.png"
            alt="Right image"
          />
        </div>
      </div>
    </section>
  </div>
</template>

<script setup></script>

<style scoped>
section {
  margin-top: 64px;
  width: 1128px;

  .body-head {
    font-family: 'Montserrat';
    font-size: 20px;
    line-height: 20px;
  }

  .body-right {
    font-family: 'Montserrat';
    font-size: 16px;
    line-height: 24px;
  }

  .grid-container {
    display: grid;
    gap: 24px;
    margin-top: 48px;

    .left-top-image-container {
      grid-column: 1;
      grid-row: 1;
      width: 649px;
      height: 413px;

      .left-top-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }

    .left-bottom-image-container {
      grid-column: 1;
      grid-row: 2;
      display: flex;
      gap: 25px;
      width: 100%;
      height: 470px;

      .left-bottom-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }

      .left-bottom-text {
        font-family: 'Montserrat';
        font-size: 16px;
        line-height: 24px;
        max-width: 264px;
        max-height: 131px;
        text-align: left;
      }
    }

    .right-image-container {
      grid-column: 2;
      grid-row: 1 / 3;

      .right-img {
        width: 456px;
        height: 907px;
        object-fit: cover;
      }
    }
  }
}
</style>
