<template>
  <div class="black" id="aboutmebody">
    <div id="left">
      <v-img id="name"
      :src="require('../assets/name.png')"></v-img>
    </div>
    <div id="right">
      <v-img id="lineart"
      :src="require('../assets/outline.png')"></v-img>
    </div>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500&display=swap');

template {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    background-color: black;
  }

  #aboutmebody {
    height: 100vh;
    display: flex;
    justify-content: center;
    padding: 50px;
    overflow-x: hidden;

  }

  #lineart{
      display: none;
  }

  #name{
    margin-top: 100px;
    height: 400px;
    width: 400px;
  }


@media only screen and (min-width: 688px) {
    #aboutmebody {
      height: 100vh;
      display: flex;
      justify-content: center;
      padding: 50px;
    }
      #lineart{
      display: none;
      }

      #name{
      display: flex;
      height: 600px;
       width: 600px;
      }
}   


@media only screen and (min-width: 992px) {
   #aboutmebody {
  height: 100vh;
  display: flex;
  justify-content: space-between;
  padding: 50px;

  }

  #lineart{
      display: flex;
      width: 300px;
      height: 350px;
      transform: scale(0.6);
  }

  #name{
    height: 400px;
    width: 400px;
  }
}

 @media only screen and (min-width: 1312px) {
  #aboutmebody {
  height: 100vh;
  display: flex;
  justify-content: space-between;
  padding: 0px;

  }

  #lineart{
      display: flex;
      width: 700px;
      height: 750px;
      transform: scale(0.8);
  }

  #name{
    height: 600px;
    width: 700px;
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