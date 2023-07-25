<template>
    <div class="main-section-three">
      <div class="cards-container-three">
        <div class="card-three" v-for="image in galleryImages" :key="image.name">
          <div class="image-container-three">
            <img :src="`/img/${image.name}`" :alt="`Gallery ${image.name}`">
          </div>
          <h4 class="card-three-title">{{ image.title }}</h4>
          <img src="/img/socials.JPG" alt="Socials">
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const galleryImages = [
    { name: 'gallery1.jpeg', title: 'A ROLL AND BANG THE FLOOR' },
    { name: 'gallery2 (1).jpeg', title: 'YOUR MELODY TO OUR MUSIC' },
    { name: 'gallery3.jpg', title: 'TOUCHING HEAVEN ON FREQUENCY' },
    { name: 'gallery4.jpg', title: 'MUSIC MAKES STRONGE BEATS' },
    { name: 'gallery5.jpg', title: 'SOUND IS THE SPARK OF TIME' },
    { name: 'gallery6.jpg', title: 'MAKE YOUR NIGHT GROOVY' }
  ];
  </script>
  
  <style>
  .main-section-three {
    text-align: center;
    padding: 0 20px; 
  }
  
  .white-text {
    color: white;
  }
  
  .cards-container-three {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 20px;
    justify-items: center;
    margin-top: 20px;
  }
  
  .card-three {
    background-color: #020202;
    padding: 10px;
    text-align: center;
    width: 100%; 
    max-width: 300px;
    margin: 0 auto;
  }
  
  .image-container-three {
    overflow: hidden;
  }
  
  .card-three img {
    width: 100%;
    height: auto;
    display: block;
  }
  
  .card-three img:last-child {
    margin-top: 10px;
  }
  
  .card-three-title {
    color: white;
  }
  </style>
  