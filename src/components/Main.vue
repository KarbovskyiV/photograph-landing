<template>
  <Header />
  <div class="center-container">
    <div class="image-container">
      <img class="hero-img" src="../assets/hero.png" alt="Hero" />

      <div class="text-over-hero-img">
        <span class="h-1">Hello, I’m</span>
        <span class="name">Victoria Zozulya</span>
        <span class="body-right">Professional <br> photographer in <br> fantasy style</span>
      </div>
    </div>

    <img class="flowers-img" src="../assets/flowers.png" alt="Flowers" />

    <div class="view-button">
      <span class="view-text">View portfolio</span>
    </div>

    <AboutMe />
  </div>
</template>

<script setup>
import Header from './Header.vue'
import AboutMe from './AboutMe.vue'
</script>

<style scoped>
.center-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;

  .image-container {
    width: 552px;
    height: 617px;
    overflow: hidden;

    .hero-img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }

  .flowers-img {
    position: absolute;
    width: 324px;
    height: 385px;
    left: 0;
    top: 498px;
  }

  .text-over-hero-img {
    .h-1 {
      position: absolute;
      top: 268px;
      left: 156px;
      font-size: 96px;
      line-height: 144px;
    }

    .name {
      position: absolute;
      top: 427px;
      right: 139px;
      font-size: 96px;
      line-height: 144px;
    }

    .body-right {
      position: absolute;
      top: 295px;
      right: 157px;
      font-family: 'Montserrat';
      font-size: 16px;
      line-height: 24px;
    }
  }

  .view-button {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 256px;
    height: 56px;
    margin-top: 95px;
    border: 1px solid #e5e1d2;
    cursor: pointer;

    .view-text {
      font-family: 'Montserrat';
      font-size: 16px;
      line-height: 24px;
    }
  }
}
</style>
