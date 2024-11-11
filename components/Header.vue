<template>
    <header class="header">
        <img src="../assets/icons/JJLogo.svg" alt="JJLogo" class="logo" />
        <div class="cityBox">
            <div class="leftButtons">
                <button class="city">
                    <img src="../assets/icons/Marker.svg" alt="Marker" />
                    <p class="nav-link">МОСКВА</p>
                </button>
                <button class="phone">
                    <img src="../assets/icons/Phone.svg" alt="Phone" />
                    <p class="nav-link2"> +7 (812) 635 22 77</p>
                </button>
            </div>
            <div class="rightButtons">
                <button class="ticketBuy">
                    <p class="ticketBuyText">КУПИТЬ БИЛЕТЫ</p>
                </button>
                <button class="holydayBuy">
                    <p class="holydayBuyText">ЗАКАЗАТЬ ПРАЗНИК</p>
                </button>
            </div>
        </div>
        <div class="headerMenu">
            <div class="headerMenuStick"></div>
            <div class="headerMenuStick2"></div>
            <div class="headerMenuStick"></div>
            <p class="headerMenuText">МЕНЮ</p>
        </div>
    </header>
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
    src: url('../assets/fonts/drukwidecyr-Medium.woff2') format('woff2'),
}

@font-face {
    font-family: 'Montserrat';
    src: url('../assets/fonts/Montserrat-Bold.ttf') format('truetype'),
}

.header {
    position: relative;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1;
    background-color: hsla(0, 0%, 100%, 0.75);
    backdrop-filter: blur(19px);
    color: white;
    padding: 12px 16px 9px 16px;
    display: flex;
}

.cityBox {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
    @media (max-width: 450px) {
        justify-content: center;
    }
}

.leftButtons {
    display: flex;
    gap: 16px;
    align-items: center;
}

@media (max-width: 450px) {
    .leftButtons {
        display: none; 
    }
}

.rightButtons {
    display: flex;
    gap: 16px;
    align-items: center;
}

.logo {
    display: block;
    width: 40px;
    height: 40px;
}

.city {
    display: flex;
    cursor: pointer;
    justify-content: space-between;
    align-items: center;
    background-color: transparent;
    margin-left: 65px;
    height: 40px;
    padding: 8px 16px 8px 16px;
    gap: 8px;
    border-radius: 30px;
    border: 2px solid #5834A4;
    transition: transform 0.3s ease-out, background-color 0.3s ease;
}

.phone {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: transparent;
    cursor: pointer;
    height: 40px;
    padding: 8px 16px 8px 16px;
    gap: 8px;
    border-radius: 30px;
    border: 2px solid #5834A4;
    transition: transform 0.3s ease-out, background-color 0.3s ease;
}

.nav-link {
    font-family: "Druk Cyr", sans-serif;
    font-size: 22px;
    font-weight: 500;
    line-height: 24px;
    letter-spacing: 0.03em;
    text-align: center;
    text-underline-position: from-font;
    color: #5834A4;
}

.nav-link2 {
    font-family: "Druk Wide Cy", sans-serif;
    font-size: 13px;
    font-weight: 500;
    line-height: 16px;
    letter-spacing: 0.03em;
    text-align: center;
    text-underline-position: from-font;
    text-decoration-skip-ink: none;
    color: #5834A4;
}

.ticketBuy {
    cursor: pointer;
    height: 40px;
    padding: 7px 32px 9px 32px;
    border-radius: 30px;
    background: #F269AF;
    border: #F269AF solid 0px;
    transition: transform 0.3s ease-out, background-color 0.3s ease;
}

.holydayBuy {
    cursor: pointer;
    height: 40px;
    padding: 7px 32px 9px 32px;
    border-radius: 30px;
    background: #ABEC20;
    border: #ABEC20 solid 0px;
    transition: transform 0.3s ease-out, background-color 0.3s ease;
}

@media (max-width: 450px) {
    .holydayBuy {
        display: none; 
    }
}

.ticketBuyText {
    font-family: "Druk Cyr", sans-serif;
    font-size: 22px;
    font-weight: 500;
    line-height: 24px;
    letter-spacing: 0.03em;
    text-align: center;
    text-underline-position: from-font;
    color: #FFFFFF;
}

.holydayBuyText {
    font-family: "Druk Cyr", sans-serif;
    font-size: 22px;
    font-weight: 500;
    line-height: 24px;
    letter-spacing: 0.03em;
    text-align: center;
    text-underline-position: from-font;
    color: #262626;
}

.ticketBuy:hover {
    transform: translateX(10px);
    background-color: #D23B8C;
}

.holydayBuy:hover {
    transform: translateX(10px);
    background-color: #91D81F;
}

.ticketBuy:active {
    animation: moveInRight 300ms ease-out;
}

.holydayBuy:active {
    animation: moveInRight 300ms ease-out;
}

.city:hover {
    transform: translateX(10px);
}

.phone:hover {
    transform: translateX(10px);
}

.city:active {
    animation: moveInRight 300ms ease-out;
}

.phone:active {
    animation: moveInRight 300ms ease-out;
}

@keyframes moveInRight {
    from {
        transform: translateX(0);
    }

    to {
        transform: translateX(10px);
    }
}

.headerMenu {
    display: flex;
    flex-direction: column;
    cursor: pointer;
    gap: 6px;
    justify-content: flex-start;
    align-items: flex-end;
    flex-grow: 1;
}

.headerMenuStick {
    display: flex;
    background: #0267FF;
    width: 32px;
    height: 4px;
}

.headerMenuStick2 {
    display: flex;
    background: #0267FF;
    width: 22px;
    height: 4px;
}

.headerMenuText {
    font-family: "Montserrat", sans-serif;
    font-size: 11px;
    font-weight: 700;
    line-height: 16px;
    letter-spacing: 0.01em;
    text-align: right;
    text-underline-position: from-font;
    text-decoration-skip-ink: none;
    color: #0267FF;
}
</style>
