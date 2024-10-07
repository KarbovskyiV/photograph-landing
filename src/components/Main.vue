<template>
  <div>
    <div class="header-container">
      <Header />
      <div class="image-container">
        <img src="../assets/header/hero.png" alt="Hero" />

        <div>
          <span class="h-1">Hello, I’m</span>
          <span class="name">Victoria Zozulya</span>
          <span class="body-right"
            >Professional <br />
            photographer in <br />
            fantasy style</span
          >
        </div>
      </div>

      <img class="flowers-img" src="../assets/header/flowers.png" alt="Flowers" />
      <div class="view-button">
        <span class="view-text">View portfolio</span>
      </div>
    </div>

    <AboutMe />
    <Portfolio />
    <Services />
  </div>
</template>

<script setup>
import AboutMe from '@/components/aboutMe/AboutMe.vue';
import Header from './Header.vue';
import Portfolio from './portfolio/Main.vue';
import Services from '@/components/services/Services.vue';
</script>

<style scoped>
.header-container {
  width: 1440px;
  height: 857px;
  margin: 0 auto;
  position: relative;

  .image-container {
    margin-top: 22px;
    margin-left: 409px;

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
      right: 156px;
      font-size: 96px;
      line-height: 144px;
    }

    .body-right {
      position: absolute;
      top: 298px;
      right: 157px;
      font-family: 'Montserrat';
    }
  }

  .flowers-img {
    position: absolute;
    width: 324px;
    top: 450px;
  }

  .view-button {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-left: 592px;
    width: 256px;
    height: 56px;
    margin-top: 95px;
    border: 1px solid #e5e1d2;
    cursor: pointer;

    .view-text {
      font-family: 'Montserrat';
    }
  }
}
</style>
