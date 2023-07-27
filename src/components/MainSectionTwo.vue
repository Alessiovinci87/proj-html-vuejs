<template>
  <div class="main-section-two">
    <div class="main-content"></div>

    <div class="full-width-image">
      <img src="/img/Video-1536x541.jpg" alt="Full Width Image">
      <div class="centered-overlay-two">
        <i class="fa-regular fa-circle-play" style="color:#f2870c;"></i>
        <h1 class="white-text-small">NEW MUSIC VIDEO</h1>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss">

.main-section-two {
  display: flex;
  align-items: center; 
}

.full-width-image {
  width: 100%;
  position: relative;
}

.full-width-image img {
  width: 100%;
  height: auto;
  display: block;
}

.centered-overlay-two {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: #ffffff;
}

.centered-overlay-two i {
  font-size: 64px;
  transition: transform 0.3s ease; 
}

.centered-overlay-two h1 {
  margin-top: 16px;
}

.centered-overlay-two i:hover {
  transform: scale(1.2); 
}
</style>
