<template>
    <div class="container">
      <div class="second-centered-text">
        <div class="title-wrapper">
          <h2 class="orange-text">WHO WE ARE</h2>
          <h1 class="white-text-one">SENSE THE JAZZ</h1>
          <div class="paragraph-container">
            <p>
              The Story Of Jazz And Blues Society Is The Story Of Determination, Passion, Idealism,
              Community, And Of Course, Music. Founded In 1985 And Incorporated In 1986, As A
              Community Based, Not-For-Profit, Charitable Arts Organization Located In Vancouver,
              British Columbia, The Society, From The Very Beginning, Has Worked Diligently To
              Establish Vancouver As A Centre For The Creation And Exchange Of Sounds And Ideas
              Between The Local, National And International Music Communities.
            </p>
          </div>
        </div>
        <button class="transparent-button">READ MORE</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'MainSectionOne',
  };
  </script>
  
  <style lang="scss">
.title-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
}


.orange-text {
  font-size: 18px;
  color: #f2870c;
}


.white-text-one {
  font-size: 50px;
  color: white;
}

.paragraph-container {
  font-size: 14px;
  text-align: center;
  margin-bottom: 30px;
  color: white; 
}

.second-centered-text {
  display: flex;
  flex-direction: column; 
  align-items: center; 
  max-width: 600px; 
  margin: 0 auto; 
  padding: 20px; 
}
  </style>
  