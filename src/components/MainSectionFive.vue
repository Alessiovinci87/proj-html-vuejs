<template>
    <div class="main-section-five">
      <div class="section-title">
        <p class="orange-text">MUSIC BLOG</p>
        <h1 class="white-text-four">BEST MUSIC BLOG</h1>
      </div>
  
      <div class="blog-images">
        <div class="blog-image">
          <img src="/img/hip_hop_wired_to_dance_make.jpg" alt="Hip Hop Wired to Dance Make">
          <p class="date orange-text"><i class="fa-regular fa-calendar"></i> 06 November 2021</p>
          <p class="blog-text">Driving Short Distances Music Is A Music Genre Taht Includes Traditionals Folk Music And The Conteporary Genre That Evolved From The Former</p>
        </div>
        <div class="blog-image">
          <img src="/img/music_business-worldwide.jpg" alt="Music Business Worldwide">
          <p class="date orange-text"><i class="fa-regular fa-calendar"></i> 27 May 2022</p>
          <p class="blog-text">Accelerate Work Andd Drive Productivity The Beatles' Experimental And Creative Freedom Led Other Bands To Experiment In Various Ways As Weel.</p>
        </div>
        <div class="blog-image">
          <img src="/img/giveaways_rock.jpg" alt="Giveaways Rock">
          <p class="date orange-text"><i class="fa-regular fa-calendar"></i> 07 May 2022</p>
          <p class="blog-text">Signs Your Car Battery Has To Be Replaced When The Dashboard Light Start Flashing, This Is A Sign The Battery Is Dying. Several Issues Arise And</p>
        </div>
      </div>
    </div>

    <div class="image-slider">
    <img v-for="image in images" :key="image" :src="`/img/${image}`" alt="Image">
  </div>
  </template>

<script setup>
const images = [
  'instagram_img1.jpg',
  'instagram_img2.jpg',
  'instagram_img3.jpg',
  'instagram_img4.jpg',
  'instagram_img5.jpg',
  'instagram_img6.jpg',
  'instagram_img7.jpg',
  'instagram_img8.jpg',
];

const currentPage = 0;
</script>
  
  <style lang="scss">
  /* Stili per il componente "MainSectionfive" */
  .main-section-five {
    text-align: center;
    background-color: #060606;
    color: white;
    padding: 40px 0;
  }

  .orange-text {
    color: #f2870c;
    font-size: 18px;
  }
  
  .section-title {
    margin-bottom: 20px;
  }
  
  .section-title h1 {
    font-size: 32px;
  }
  
  .blog-images {
    display: flex;
    justify-content: space-between;
  }
  
  .blog-image {
    width: 30%;
    background-color: #161616;
    padding: 10px;
    text-align: center;
  }
  
  .blog-image img {
    width: 100%;
    height: auto;
    display: block;
  }
  
  .date {
    margin-top: 10px;
    font-size: 14px;
  }
  
  .blog-text {
    margin-top: 10px;
    color: white;
  }

  .main-section-five {
  text-align: center;
  padding: 40px 0;
}

.orange-text {
  color: #f2870c;
  font-size: 18px;
}

.image-slider {
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

img {
  max-width: 100%;
  height: auto;
  margin-right: 10px; /* Aggiungi spazio tra le immagini */
}
  </style>
  