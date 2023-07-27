<template>
    <div class="main-section-four">
      <div class="parallax-image">
        <img src="/img/cms_parallax.jpg" alt="Parallax Image">
        <div class="centered-overlay-four">
          <h4 class="orange-text">INSTRUMENTAL ROCK</h4>
          <h1 class="white-text-large">ALBUM OUT NOW</h1>
          <button class="transparent-button">READ MORE</button>
        </div>
      </div>
    </div>
   

    <div class="counter-parallax" 
    style="background-image: url('/img/counter_parallax.jpg');">
      <div class="counter-container">
        <div class="card-four">
          <img src="/img/image (13).svg" alt="Image 13">
          <h3 class="counter-number">163</h3>
          <p class="counter-label">CONCERT</p>
        </div>
        <div class="card-four">
          <img src="/img/image (14).svg" alt="Image 14">
          <h3 class="counter-number">145</h3>
          <p class="counter-label">HAPPY CLIENTS</p>
        </div>
        <div class="card-four">
          <img src="/img/image (15).svg" alt="Image 15">
          <h3 class="counter-number">72</h3>
          <p class="counter-label">MUSIC AWARDS</p>
        </div>
        <div class="card-four">
          <img src="/img/image (16).svg" alt="Image 16">
          <h3 class="counter-number">182</h3>
          <p class="counter-label">TOTAL SONG</p>
        </div>
      </div>
    </div>
 
  </template>
  
  <style lang="scss">

  
  .main-section-four {
    text-align: center;
  }
  
  .parallax-image {
    position: relative;
    overflow: hidden;
    width: 100%;
    height: 100vh;
  }
  
  .parallax-image img {
    margin-top: 150px;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  
  .centered-overlay-four {
    position: absolute;
    top: 60%;
    left: 10%;
    transform: translateY(-50%);
    text-align: left;
    color: white;
    width: 100%;
    padding: 20px;
    box-sizing: border-box;
  }
  

  .main-section-five {
  text-align: center;
}

.parallax-image {
  position: relative;
  overflow: hidden;
  width: 100%;
  height: 100vh;
}

.parallax-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.centered-overlay {
  position: absolute;
  top: 50%;
  left: 0;
  transform: translateY(-50%);
  text-align: left;
  color: #ffffff;
  width: 100%;
  padding: 20px;
  box-sizing: border-box;
}



.transparent-button {
  font-size: 16px;
  background-color: transparent;
  border: 2px solid #f2870c;
  color: #ffffff;
  padding: 10px 20px;
  cursor: pointer;
  transition: background-color 0.3s ease, color 0.3s ease;
}

.transparent-button:hover {
  background-color: #f2870c;
  color: #ffffff;
}

.counter-container {
  display: flex;
  justify-content: space-around; 
  padding: 111px;
}

.counter-parallax {
  height: 50vh;
}

.card-four {
  background-color: rgba(6, 6, 6, 0.5);
  padding: 20px;
  text-align: center;
  width: 200px;
}

.card-four img {
  width: 80px;
  height: 80px;
  display: block;
  margin: 0 auto;
  filter: brightness(0) invert(1);
}

.counter-number {
  font-size: 40px;
  color: #ffffff;
}

.counter-label {
  font-size: 18px;
  color: #ffffff;
}
  </style>
  