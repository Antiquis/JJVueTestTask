<template>
  <footer class="footer">
    <img src="../assets/icons/JJFooterLogo.svg" alt="jjFooterLogo">
    <div class="cityFooterWrapper">
      <span class="cityFooter">+7 (495) 181 22 77</span>
      <p class="cityFooterP">(МОСКВА, ТВЕРЬ)</p>
      <span class="cityFooter">+7 (812) 635 22 77</span>
      <p class="cityFooterP">(САНКТ-ПЕТЕРБУРГ)</p>
    </div>
    <div class="socialWrapper">
      <img src="../assets/icons/Vk.svg" alt="Vk" class="socialImage">
      <img src="../assets/icons/Telegram.svg" alt="Telegram" class="socialImage">
      <img src="../assets/icons/JJSocial.svg" alt="JJSocial" class="socialImage">
    </div>
    <div class="siteText">
      <span>Joki Joya ©</span>
      <p>2023</p>
      <span>joki-joya.ru</span>
    </div>
    <button class="upButton" @click="scrollToTop">
      Наверх
      <img src="../assets/icons/ArrowFooter.svg" alt="ArrowFooter" class="ArrowFooter">
    </button>
  </footer>
</template>

<script setup lang="ts">
const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: 'smooth'
  });
};
</script>

<style scoped lang="scss">
@font-face {
  font-family: 'Druk Wide Cy';
  src: url('../assets/fonts/drukwidecyr-Medium.woff2') format('woff2');
}

@font-face {
  font-family: 'Nunito Sans';
  src: url('../assets/fonts/NunitoSans-Regular.ttf') format('truetype');
}

.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  padding: 48px 112px 48px 112px;
  background: #F269AF;
  color: white;
  text-align: center;
  margin-top: auto;
  z-index: 1;
  @media (max-width:450px) {
    flex-direction: column;
    gap: 15px;
  }
}

.cityFooterWrapper {
  display: flex;
  flex-direction: column;
}

.socialWrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 256px;
}

.socialImage {
  height: 32px;
  width: 32px;
}

.cityFooter {
  font-family: "Druk Wide Cy", sans-serif;
  color: #ABEC20;
  font-size: 13px;
  font-weight: 500;
  line-height: 16px;
  letter-spacing: 0.03em;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

.cityFooterP {
  font-family: "Druk Wide Cy", sans-serif;
  font-size: 13px;
  font-weight: 500;
  line-height: 16px;
  letter-spacing: 0.03em;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;

}

.siteText {
  font-family: "Nunito Sans", sans-serif;
  font-size: 12px;
  font-weight: 900;
  line-height: 16px;
  letter-spacing: -0.01em;
  text-align: right;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

.upButton {
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  width: 176px;
  height: 64px;
  padding: 9px 26px 9px 26px;
  gap: 10px;
  border-radius: 62px;
  border: 2px solid #FFFFFF;
  background-color: transparent;
  font-family: "Druk Cyr", sans-serif;
  font-size: 22px;
  font-weight: 500;
  line-height: 24px;
  letter-spacing: 0.03em;
  text-align: center;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: #FFFFFF;
}

.upButton:hover {
  opacity: 0.8;
}

</style>