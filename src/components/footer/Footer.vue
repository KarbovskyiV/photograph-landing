<template>
  <div class="footer-container">
    <div class="footer-left">Zozulya</div>

    <div class="footer-center">
      <div class="footer-links">
        <span>About Me</span>
        <span>Portfolio</span>
        <span>Services</span>
        <span>Reviews</span>
        <span>Contacts</span>
      </div>

      <div class="footer-contacts">
        <div><i class="bi bi-envelope"></i><span>emailemail@gmail.com</span></div>
        <div><i class="bi bi-telephone"></i><span>+380951234567</span></div>
        <div><i class="bi bi-geo-alt"></i><span>Kyiv</span></div>
      </div>
    </div>

    <div class="footer-right">All rights reserved.</div>
  </div>
</template>

<style scoped>
.footer-container {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 257px auto 0 auto;
  max-width: 1440px;
  width: 100%;
  background-color: #b7b597;
  color: #0c1813;
  font-family: 'Montserrat';

  .footer-center {
    display: flex;
    gap: 111px;
    padding-top: 59px;
    padding-bottom: 45px;

    .footer-links {
      display: flex;
      flex-direction: column;
    }

    .footer-contacts {
      display: flex;
      flex-direction: column;
      gap: 16px;

      div {
        display: flex;
      }

      i {
        font-size: 24px;
        padding-right: 24px;
      }
    }
  }

  .footer-left {
    align-self: flex-start;
    padding-right: 204px;
    padding-top: 29px;
    font-family: 'Playfair Display';
    font-size: 40px;
    font-weight: 600;
    line-height: 60px;
  }

  .footer-right {
    padding-left: 198px;
    padding-top: 105px;
  }
}
</style>
