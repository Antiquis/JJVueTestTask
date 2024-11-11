<template>
  <div id="app">
    <Header />
    <div class="lineGradient"></div>
    <div class="main-content">
      <Sidebar />
      <div class="content-area">
        <Body>
          <NuxtPage />
        </Body>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script setup lang="ts">
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';
import Body from '~/components/Body.vue';
import Sidebar from '@/components/Sidebar.vue';
</script>

<style scoped lang="scss">

#app{
  height: 3550px;
  background-image: url("./assets/icons/Expect2.jfif"); 
  background-size: cover;
  background-position: center;
  background-repeat: repeat;
  display: flex;
  flex-direction: column;
  @media (max-width: 450px) {
    width: 700px;
    height: 4750px;
  }
}

.sidebar-toggle {
  display: none;
}

@media (max-width: 768px) {
  .sidebar-toggle {
    display: block;
    background-color: #333;
    color: white;
    font-size: 30px;
    position: fixed;
    top: 20px;
    left: 20px;
    z-index: 10;
  }
}

.main-content {
  display: flex;
  position: absolute;
  top: 0;
  left: 0;
  height: 100vh;
  display: flex;
  z-index: 0;
}

.content-area {
  padding: 0px 0px 0px 48px;
}

.sidebar.open {
  left: 0;
}

@media (max-width: 768px) {
  .content-area {
    margin-left: 0;
  }
}

.lineGradient {
  display: grid;
  background: linear-gradient(227.56deg, #FDF398 -0.59%, #F7BE87 22.84%, #E5637D 45.63%, #E84BBA 65.89%, #9310D8 99.13%);
  height: 3.01px;
  z-index: 2;
}
</style>
