<template>
  <div class="main-content">
    <div class="background-wrapper">
      <img class="background-image" src="/img/image (1).png" alt="Background Image">
      <div class="centered-text">
        <div class="title-wrapper">
          <h2 class="orange-text">INSTRUMENTAL ROCK</h2>
          <h1 class="white-text-large">MUSIC IN THIS VIDEO</h1>
        </div>
        <button class="transparent-button">READ MORE</button>
      </div>
    </div>
  </div>
  <div class="main-container">
    <div class="image-container">
      <div class="cards-container">
        <div class="card">
          <div class="card-content">
            <img src="icon/speaker.svg" alt="Original Ideas">
            <h5>ORIGINAL IDEAS</h5>
            <p>
              Contrary Popular Belief, Lorem Ipsum Not Simply Ipsum Random Text
            </p>
          </div>
        </div>
        <div class="card">
          <div class="card-content">
            <img src="icon/disc.svg" alt="Music Studio">
            <h5>MUSIC STUDIO</h5>
            <p>
              Contrary Popular Belief, Lorem Ipsum Not Simply Ipsum Random Text
            </p>
          </div>
        </div>
        <div class="card">
          <div class="card-content">
            <img src="icon/headphones.svg" alt="Acoustic Covers">
            <h5>ACOUSTIC COVERS</h5>
            <p>
              Contrary Popular Belief, Lorem Ipsum Not Simply Ipsum Random Text
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
  
</template>

<script setup>

</script>

<style lang="scss">

* {
  font-family: 'Oswald', sans-serif;
}

.main-content {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}


.background-wrapper {
  position: relative;
  width: 100%;
  height: 100%;
}


.background-image {
  width: 100%;
  height: 100%;
}


.centered-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}


.title-wrapper {
  display: flex;
  align-items: center;
}


.orange-text {
  margin: 0;
  font-size: 18px;
  color: #f2870c;
}


.white-text-large {
  margin: 20px 0;
  font-size:110px;
  color: #ffffff;
  white-space: nowrap;
}


.transparent-button {
  width: 200px;
  font-size: 16px;
  background-color: transparent;
  border: 2px solid #f2870c;
  color: #ffffff;
  padding: 10px 20px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.transparent-button:hover {
  background-color: #f2870c;
}

.main-container {
  height: 100%;
}

.image-container {
  position: relative;
  height: 100%;
  display: flex;
  align-items: flex-end;

}

img {
  width: 100%;
  height: auto;
  display: block;

}

.cards-container {
  display: flex;
  justify-content: space-between;
  width: 100%;
  padding: 0 50px;
  box-sizing: border-box;
}

.card {
  margin: 10px;
  background-color: #161616;
  padding: 30px;
  flex: 1;
  text-align: center;
  margin-top: -40px;
  position: relative;
  bottom: 100px;
}

.card-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;

}

.card img {
  width: 80px;
  margin-bottom: 10px;
  filter: brightness(0) invert(1);
}


.card p {
  color: #ffffff;
}

.card h5 {
  color: white;
  font-size: 25px;
  margin:20px;
}

@media (max-width: 768px) {
  .cards-container {
    flex-direction: column;
    align-items: center;
  }

  .card {
    margin-top: 0;
  }

  .card img {
    width: 60px;
  }
}


</style>