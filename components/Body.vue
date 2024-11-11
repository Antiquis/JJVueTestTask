<template>

  <body class="body-container">
    <img src="../assets/icons/MainImage.svg" alt="MainImage" class="mainImage">
    <div class="text-container">
      <div class="imgTextWrapper">
        <span class="oText">O </span>
        <span class="jjText">JOKI JOYA</span>
        <div class="starsImgContainer">
          <img src="../assets/icons/JJStar.svg" alt="JJStar" class="jjStarImg">
          <img src="../assets/icons/JJStar.svg" alt="JJStar" class="jjStarImg">
          <img src="../assets/icons/JJStar.svg" alt="JJStar" class="jjStarImg">
        </div>
      </div>
      <img src="../assets/icons/Welcome.svg" alt="Welcome" class="welcomeImg">
    </div>
    <div class="wrapperWrapperov">
      <div class="verticalWrapper">
        <div class="verticalContainer">
          <img src="../assets/icons/SnowImage.svg" alt="SnowImage" class="SnowImage">
          <span class="verticalText">JJSHOW</span>
        </div>
        <div class="verticalContainer">
          <img src="../assets/icons/SnowImage.svg" alt="SnowImage" class="SnowImage">
          <span class="verticalText">CELEBRATE</span>
        </div>
        <div class="verticalContainer">
          <img src="../assets/icons/SnowImage.svg" alt="SnowImage" class="SnowImage">
          <span class="verticalText">BIRTHDAY</span>
        </div>
        <div class="verticalContainer">
          <img src="../assets/icons/SnowImage.svg" alt="SnowImage" class="SnowImage">
          <span class="verticalText">QUESTS</span>
        </div>
      </div>
      <div class="ourParksWrapper">
        <span class="ourParksText">НАШИ ПАРКИ:</span>
        <img src="../assets/icons/Rhomb2.svg" alt="Rhomb" class="rhombImg">
      </div>
      <div class="jjInfoTextContainer">
        <span class="jjInfoText">
          <span class="jjInfoH3">Первый парк развлечений Joki Joya</span> открылся в августе 2014 года в
          Санкт-Петербурге. Сегодня бренд Joki Joya является лидером
          индустрии детских развлечений в России и состоит из 28 парков в 3 городах: 17 в Москве и Московской области,
          10 в Санкт-Петербурге и 1 в Твери.
          На территории каждого парка размещено более 30 аттракционов в игровой зоне, семейный ресторан с детским и
          взрослым меню, индивидуальные банкетные комнаты для проведения праздников.
        </span>
      </div>
      <div class="jjInfoWrapper">
        <span class="jjInfoText2">
          <p>Площадь парков от 2000 до 6000 квадратных метров в зависимости от ТРЦ.</p>
          <p>Также Joki Joya занимается организацией праздников «под ключ»: детские дни рождения, выпускные детского
            сада или школы, Новый Год, корпоративные праздники.</p>
        </span>
        <button class="lookAdres">
          ПОСМОТРЕТЬ АДРЕСА
          <img src="../assets/icons/Arrow.svg" alt="Arrow" class="lookAdresArrow" />
        </button>
      </div>
    </div>
    <div class="gridWrapperSecond">
      <div class="ourParksWrapper">
        <span class="ourParksText">ПРАЗДНИКИ У НАС:</span>
        <img src="../assets/icons/Flower.svg" alt="Rhomb" class="rhombImg">
      </div>
      <div class="jjInfoTextContainer">
        <span class="jjInfoText2">
          <p>Праздник можно отметить в индивидуальной банкетной комнате, расписанной профессиональными художниками
            вручную под тематику популярных фильмов или мультфильмов, либо в семейном ресторане.</p>
          <p>Что мы имеем в виду, когда говорим про организацию праздников «под ключ»? За каждым праздником мы
            закрепляем личного банкетного менеджера, который будет курировать ваш праздник.</p>
        </span>
      </div>
      <div class="jjInfoWrapper">
        <span class="jjInfoText2">
          <p>В нашей базе более 300 аниматоров, шоу-программ и квестов, которые помогут создать особую атмосферу
            праздника. Украсят ваш праздник профессиональные аквагримеры, лучшие торты на заказ, а также фото — и
            видеосъемка.</p>
          <p> <span class="jjInfoH3">Joki Joya</span> - это целая история про детей и их родителей. История, которая
            помогает семьям объединяться, окунаться с головой в детство и проводить время вместе, забывая о повседневной
            суёте.</p>
        </span>
      </div>
    </div>
    <div class="gridFacts">
      <button class="factsButton">
        <img src="../assets/icons/Card.svg" alt="Image 1" class="factImage">
      </button>
      <button class="factsButton">
        <img src="../assets/icons/Card2.svg" alt="Image 2" class="factFixImage">
      </button>
      <button class="factsButton">
        <img src="../assets/icons/Card3.svg" alt="Image 3" class="factImage">
      </button>
      <button class="factsButton">
        <img src="../assets/icons/Card4.svg" alt="Image 4" class="factImage">
      </button>
      <button class="factsButton">
        <img src="../assets/icons/Card5.svg" alt="Image 5" class="factFixImage">
      </button>
      <button class="factsButton">
        <img src="../assets/icons/Card6.svg" alt="Image 6" class="factImage">
      </button>
      <button class="factsButton">
        <img src="../assets/icons/Card7.svg" alt="Image 7" class="factImage">
      </button>
    </div>
    <slot />
  </body>
</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">
@font-face {
  font-family: 'Druk Cyr';
  src: url('../assets/fonts/DrukCyr-Medium.ttf') format('truetype');
}

@font-face {
  font-family: 'Druk Wide Cy';
  src: url('../assets/fonts/drukwidecyr-Medium.woff2') format('woff2');
}

@font-face {
  font-family: 'Nunito Sans';
  src: url('../assets/fonts/NunitoSans-Regular.ttf') format('truetype');
}

.body-container {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  color: #333;
  width: 100%;
}

.mainImage {
  min-width: 1616px;
  width: 90%;
  height: auto;
  border-radius: 32px;
  @media (max-width: 450px) {
    max-width: 600px;
    min-width: 0px;
  }
}

.text-container {
  display: flex;
  gap: 15px;
  align-items: center;
  padding-top: 40px;
  width: 90%;
  justify-content: space-between;
  @media (max-width:450px) {
  }
}

.oText {
  font-family: "Druk Wide Cy", sans-serif;
  font-size: 73px;
  font-weight: 500;
  line-height: 72px;
  color: #000000;
}

.jjText {
  font-family: "Druk Wide Cy", sans-serif;
  font-size: 73px;
  font-weight: 500;
  line-height: 72px;
  color: #0267FF;
}

.starsImgContainer {
  display: inline-flex;
  gap: 19px;
}

.imgTextWrapper {
  display: flex;
  gap: 27px;
  align-items: center;
}

.jjInfoText {
  display: block;
  font-family: "Nunito Sans", sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: -0.01em;
  text-align: left;
  color: #000000;
}

.jjInfoText2 {
  font-family: "Nunito Sans", sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: -0.01em;
  text-align: left;
  color: #000000;
}

.jjInfoH3 {
  font-family: "Nunito Sans", sans-serif;
  font-size: 16px;
  font-weight: 900;
  line-height: 24px;
  letter-spacing: -0.01em;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;

}

.wrapperWrapperov {
  display: grid;
  grid-template-columns: 80px 170px 1fr 1fr;
  gap: 103px;
  margin-top: 150px;
  width: 90%;
}

.verticalWrapper {
  display: flex;
  flex-direction: row;
  gap: 20px;
  align-items: flex-end;
  height: 110px;
  width: 90px;
  transform: rotate(90deg);
}

.verticalContainer {
  display: flex;
  align-items: center;
  position: relative;
  border: none;
  gap: 40px;
  padding-right: 40px;
}

.verticalText {
  color: #000000;
  font-family: "Druk Cy", sans-serif;
  font-size: 84px;
  font-weight: 500;
  line-height: 84px;
  transform: rotate(180deg);
}

.SnowImage {
  width: 64px;
  height: 72px;
}

.ourParksText {
  font-family: "Druk Wide Cy", sans-serif;
  font-size: 13px;
  font-weight: 500;
  line-height: 16px;
  letter-spacing: 0.03em;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

.ourParksWrapper {
  display: flex;
  justify-content: space-between;
  flex-direction: column;
}

.rhombImg {
  height: 128px;
  width: 128px;
}

.lookAdres {
  display: flex;
  align-items: center;
  cursor: pointer;
  margin-top: 48px;
  padding: 11px 21.25px 13px 17.5px;
  gap: 12.5px;
  border-radius: 48px;
  border: 2px solid #000000;
  font-family: "Druk Cyr", sans-serif;
  font-size: 22px;
  font-weight: 500;
  line-height: 24px;
  background-color: transparent;
  letter-spacing: 0.03em;
  text-align: center;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;

}

.lookAdresArrow {
  width: 32px;
  height: 17.36px;
}

.jjInfoTextWrapper {
  display: flex;
}

.jjInfoTextContainer {
  justify-self: center;
}

.jjInfoText2 p {
  margin: 0 0 16px 0;
  font-family: "Nunito Sans", sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: -0.01em;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;

}

.gridWrapperSecond {
  display: grid;
  grid-template-columns: 170px 1fr 1fr;
  gap: 103px;
  margin-top: 126px;
  padding-left: 183px;
  width: 90%;
}

.gridFacts {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  width: 90%;
  padding-left: 183px;
  padding-top: 143px;
  @media (max-width: 450px) {
    grid-template-columns: 1fr; /* Устанавливаем одну колонку */
  }
}

.factImage {
  width: 100%;
  height: auto;
  object-fit: cover;
  transition: transform 0.3s ease;
  pointer-events: none;
  @media (max-width: 450px) {
    height: 240px;
    width: 344px
  }
}

.factFixImage {
  width: 100%;
  height: auto;
  object-fit: cover;
  transition: transform 0.3s ease;
  pointer-events: none;
  @media (max-width: 450px) {
    height: 240px;
    width: 344px
  }
}

.factsButton {
  border: none;
  cursor: pointer;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background: transparent;
  @media (max-width: 450px) {
    height: 240px;
    width: 344px
  }
}

.factsButton:hover .factImage {
  transform: scale(1.05); 
}

.factsButton:hover .factFixImage {
  transform: scale(1.05);
}

.welcomeImg {
  display: flex;

}
</style>
