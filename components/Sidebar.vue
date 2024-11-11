<template>
  <div class="sidebar">
    <div class="dropdown">
      <button @click="toggleMenu" class="dropdownKek">
        <img src="../assets/icons/MenuArrow.svg" alt="MenuArrow" class="MenuArrow">
        <p class="dropDownText">ПАРКИ</p>
        <div v-if="isOpen" class="dropdown-menu">
          <a href="#" class="dropdown-item">Опция 1</a>
          <a href="#" class="dropdown-item">Опция 2</a>
          <a href="#" class="dropdown-item">Опция 3</a>
        </div>
      </button>
      <button @click="toggleMenu" class="dropdownKek">
        <img src="../assets/icons/MenuArrow.svg" alt="MenuArrow" class="MenuArrow">
        <p class="dropDownText">ПРАЗДНИКИ</p>
        <div v-if="isOpen" class="dropdown-menu">
          <a href="#" class="dropdown-item">Опция 1</a>
          <a href="#" class="dropdown-item">Опция 2</a>
          <a href="#" class="dropdown-item">Опция 3</a>
        </div>
      </button>
      <button @click="toggleMenu" class="dropdownKek">
        <img src="../assets/icons/MenuArrow.svg" alt="MenuArrow" class="MenuArrow">
        <p class="dropDownText">РЕСТОРАНЫ</p>
        <div v-if="isOpen" class="dropdown-menu">
          <a href="#" class="dropdown-item">Опция 1</a>
          <a href="#" class="dropdown-item">Опция 2</a>
          <a href="#" class="dropdown-item">Опция 3</a>
        </div>
      </button>
      <button @click="toggleMenu" class="dropdownKek">
        <img src="../assets/icons/MenuArrow.svg" alt="MenuArrow" class="MenuArrow">
        <p class="dropDownText">АФИША</p>
        <div v-if="isOpen" class="dropdown-menu">
          <a href="#" class="dropdown-item">Опция 1</a>
          <a href="#" class="dropdown-item">Опция 2</a>
          <a href="#" class="dropdown-item">Опция 3</a>
        </div>
      </button>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const isOpen = ref(false);

function toggleMenu() {
  isOpen.value = !isOpen.value;
}
</script>

<style scoped lang="scss">
@font-face {
  font-family: 'Druk Cyr';
  src: url('../assets/fonts/DrukCyr-Medium.ttf') format('truetype');
}

.sidebar {
  background: #A66EFF;
  color: white;
  padding: 20px;
  padding-top: 70px;
  display: flex;
  position: relative;
  height: 3500px;
}

.dropdown {
  display: flex;
  position: relative;
  flex-direction: column;
  justify-content: space-between;
  padding-top: 40px;
  height: 30%;
}

.dropdownKek {
  display: flex;
  align-items: center;
  position: relative;
  width: 32px;
  gap: 13px;
  background: #A66EFF;
  border: none;
  cursor: pointer;
  transform: rotate(90deg);
}

.MenuArrow {
  height: 16px;
  width: 16px;
  transform: rotate(270deg);
}

.dropdown-menu {
  display: flex;
  flex-direction: column;
  position: absolute;
  bottom: 175%;
  right: -300%;
  background-color: white;
  border: 1px solid #ddd;
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
  min-width: 160px;
  padding: 8px 0;
  z-index: 1;
  transform: rotate(270deg);
}

.dropDownText {
  color: white;
  font-family: "Druk Cyr", sans-serif;
  font-size: 24px;
  font-weight: 500;
  line-height: 24px;
  letter-spacing: 0.03em;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  transform: rotate(180deg);
}

.dropdown-item {
  padding: 12px 16px;
  color: black;
  text-decoration: none;

  &:hover {
    background-color: #f1f1f1;
  }
}
</style>
