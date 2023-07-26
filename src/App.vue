<template>
  <div>
    <HeaderNavbar />
    <Main />
    <MainSectionOne/>
    <MainSectionTwo />
    <MainSectionThree />
    <MainSectionFour/>
    <MainSectionFive/>
    <Footer />
  </div>
</template>

<script setup>
import HeaderNavbar from './components/HeaderNavbar.vue';
import Main from './components/Main.vue';
import MainSectionOne from './components/MainSectionOne.vue';
import MainSectionTwo from "./components/MainSectionTwo.vue";
import MainSectionThree from "./components/MainSectionThree.vue";
import MainSectionFour from "./components/MainSectionFour.vue";
import MainSectionFive from "./components/MainSectionFive.vue";
import Footer from './components/Footer.vue';
</script>

<style lang="scss">
@import '@fortawesome/fontawesome-free/css/all.min.css';



body {
  background-color: black;
  font-family: 'Roboto', sans-serif;
}

.container {
  margin: 0 auto;
  padding: 0 20px;
}
</style>
