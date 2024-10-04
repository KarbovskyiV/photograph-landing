<template>
  <div>
    <section>
      <div class="d-flex justify-content-between">
        <span class="body-head">PORTRAITS</span>
        <span class="body-right">Make magical dreams come true</span>
      </div>

      <div class="grid-container">
        <div class="left-image-container">
          <img class="left-img" src="../../assets/portfolio/firstSection/left-img.png" alt="Left image" />
        </div>

        <div class="top-right-image-container">
          <img
            class="top-right-img"
            src="../../assets/portfolio/firstSection/right-top-img.png"
            alt="Top right image"
          />
        </div>

        <div class="bottom-right-image-container">
          <img
            class="bottom-right-img"
            src="../../assets/portfolio/firstSection/right-bottom-img.png"
            alt="Bottom right image"
          />
          <div class="bottom-right-text">
            Each session is a journey where we transform your unique essence into a work of art. Whether you wish to
            embody a mythical hero, a whimsical creature, or a timeless legend, I craft bespoke portraits that capture
            your true spirit with a touch of enchantment
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup></script>

<style scoped>
section {
  margin-top: 48px;
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

    .left-image-container {
      grid-row: 1 / 3;
      width: 455px;
      height: 907px;

      .left-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }

    .top-right-image-container {
      grid-column: 2;
      grid-row: 1;
      width: 649px;
      height: 413px;

      .top-right-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }

    .bottom-right-image-container {
      grid-column: 2;
      grid-row: 2;
      display: flex;
      gap: 25px;
      width: 100%;

      .bottom-right-img {
        width: 360px;
        height: 470px;
        object-fit: cover;
      }

      .bottom-right-text {
        font-family: 'Montserrat';
        font-size: 16px;
        line-height: 24px;
        max-width: 264px;
        max-height: 213px;
        text-align: left;
      }
    }
  }
}
</style>
