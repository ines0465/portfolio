<template>
  <div class="black" id="aboutmebody">
    <div id="left">
      <h1 id="name">INES ADA<br>PIĄTKOWSKA</h1>
      <v-img id="lines"
      :src="require('../assets/lines.png')"></v-img>
      <h3 id="job">CREATIVE DIRECTOR<br>GRAPHIC DESIGNER</h3>
    </div>
    <div id="right">
      <v-img id="img"
      :src="require('../assets/hero.png')"></v-img>
    </div>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500&display=swap');

template {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    background: black;
  }

#aboutmebody {
  height: 100vh;
  display: flex;
  justify-content: center;
  padding: 150px;
}

#img{
  display: flex;
    width: 300px;
    height: 200px;
}

#name{
  font-size: 4em;
  text-transform: uppercase;
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: white;
    margin-right: 500px;
}

#job {
  margin-top: 0px;
  font-size: 20px;
  text-transform: uppercase;
  letter-spacing: 5px;
  color: white;
}

#lines{
  width: 220px;
  margin-top: 20px;
  display: none;
}

  @media only screen and (min-width: 749px) {
    #hero {
      height: 100vh;
      display: flex;
      justify-content: space-between;
      padding: 150px 50px;

      #name{
        font-size: 4em;
        letter-spacing: 10px;
        text-transform: uppercase;
        color: white;
      }

      #job {
        margin-top: 20px;
        font-size: 3em;
        text-transform: lowercase;
        letter-spacing: 2px;
        color: white;
      }

      #lines{
        width: 250px;
        margin-top: 20px;
      }

        #img{
          display: flex;
          width: 400px;
          height: auto;
        }
    }   
  }

@media only screen and (min-width: 1100px) {
  #hero {
  height: 100vh;
  display: flex;
  justify-content: space-between;
  padding: 150px;
  }
}

</style>

<script>

export default {
  name: 'AboutMe',
  

  components: {
    
  },

  data: () => ({
    //
  }),
};
</script>