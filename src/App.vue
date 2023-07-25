
<template>
  <div>
    <Navbar />
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
import Navbar from './components/Navbar.vue';
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
@import './styles/reset.sass';


body {
  background-color: black;
  font-family: 'Roboto', sans-serif;
}

.container {
  margin: 0 auto;
  padding: 0 20px;
}
</style>
