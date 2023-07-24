
<template>
  <div>
    <Navbar />
    <Header />
    <main>

    </main>
    <Footer />
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue';
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
</script>

<style lang="scss">
@import '@fortawesome/fontawesome-free/css/all.min.css';
@import './styles/reset.sass';


body {
  font-family: 'Roboto', sans-serif;
  line-height: 1.6;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
</style>
