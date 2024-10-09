<template>
  <div class="connection-container">
    <BaseHeader name="Get in touch with me" />
    <section>
      <div class="text-container">
        <div class="info-text">
          <p class="description">
            Whether you have a question, want to discuss ideas, or are ready to book your enchanting photo shoot, I’m
            here to help.
          </p>
          <p>Reach out to me and let’s start crafting your story.</p>
        </div>
      </div>
      <form action="#">
        <div class="mb-3">
          <input type="email" placeholder="Email" class="form-control" />
        </div>
        <div class="row">
          <div class="mb-3 col-6">
            <input type="text" placeholder="Name" class="form-control" />
          </div>
          <div class="mb-3 col-6">
            <input type="text" placeholder="Phone" class="form-control" />
          </div>
        </div>
        <div class="mb-3">
          <input type="text" placeholder="Message" class="form-control" />
        </div>

        <ButtonWithHover name="Send" />
      </form>

      <div class="image-container">
        <img class="image-cover" src="../../assets/getInTouchWithMe/open-tulip.png" alt="Open tulip" />
      </div>
    </section>
  </div>
</template>

<script setup>
import BaseHeader from '@/components/headers/BaseHeader.vue';
import ButtonWithHover from '@/components/buttons/ButtonWithHover.vue';
</script>

<style scoped>
@import '@/assets/global.css';

.connection-container {
  display: flex;
  align-items: center;
  flex-direction: column;
  margin-top: 120px;

  section {
    display: flex;
    justify-content: space-between;
    max-width: 1128px;
    width: 100%;
    margin-top: 64px;

    .text-container {
      width: 479px;
      margin-top: 80px;

      .info-text {
        width: 264px;
        font-family: 'Montserrat';

        .description {
          font-family: 'Montserrat';
          margin: 0 0 10px;
        }
      }
    }

    form {
      width: 649px;

      .form-control {
        background-color: #0c1813;
        color: #e5e1d2;
        border-width: 1px 0;
        border-radius: 0;
        border-color: #e5e1d2;
        padding: 23px 16px;
      }

      .form-control:focus {
        border-color: #e5e1d2;
        box-shadow: none;
      }

      .form-control::placeholder {
        font-size: 14px;
        line-height: 21px;
        font-family: 'Montserrat';
        color: #e5e1d2;
        transition: color 0.8s ease-out;
      }

      .form-control:focus::placeholder {
        color: transparent;
      }
    }

    .image-container {
      position: absolute;
      width: 192px;
      height: 208px;
      margin-top: 229px;
      margin-left: 192px;
    }
  }
}
</style>
