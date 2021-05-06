<template>
  <div class="black" id="gallery">
    <v-row id="mywork">
      <h1 id="myworktitle">MY WORK</h1>
    </v-row>
    <v-row id="row">
      <v-col id="column">
        <v-img class="image" :src="require('/src/assets/art1.png')" />
        <v-img class="image" :src="require('/src/assets/art2.png')" />
        <v-img class="image" :src="require('/src/assets/art3.png')" />
      </v-col>

    </v-row>

     <v-row id="row">

       <v-col id="column">
         <v-img class="image" :src="require('/src/assets/art4.png')" />
        <v-img class="image" :src="require('/src/assets/art5.png')" />
        <v-img class="image" :src="require('/src/assets/art6.png')" />
        
      </v-col>
      
    </v-row>

    <v-row id="row">

       <v-col id="column">
         <v-img class="image" :src="require('/src/assets/art7.png')" />
        <v-img class="image" :src="require('/src/assets/art8.png')" />
        <v-img class="image" :src="require('/src/assets/art9.png')" />
        
      </v-col>
      
    </v-row>



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

#gallery {
  height: auto;
  width: 100vw;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  padding: 20px;

}
#mywork{
  width: 100%;
  justify-content: center;
  margin-top: 40px;
}
#row{
  height: 100%;
  margin: 0;
  width: 100%;
}
#column{
  width: 30%;
  height: 20%;
  height: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: row;
  margin: 0;
}
.image{
  width: 10%;
  height: 30vh;
  margin: 1vw;
}

#myworktitle{
  color: transparent;
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #FFDD00;
  font-size: 40px;
}
@media only screen and (min-width: 688px) {
  #gallery {
  height: auto;
  width: 100vw;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  padding: 20px;

  }
  #mywork{
    width: 100%;
    justify-content: center;
    margin-top: 40px;
  }
  #row{
    height: 100%;
    margin: 0;
    width: 100%;
  }
  #column{
    width: 30%;
    height: 20%;
    height: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: row;
    margin: 0;
  }
  .image{
    width: 10%;
    height: 50vh;
    margin: 1vw;
  }

  #myworktitle{
    color: transparent;
    -webkit-text-stroke-width: 2px;
    -webkit-text-stroke-color: #FFDD00;
    font-size: 60px;
  }
}    
</style>

<script>

export default {
  name: 'Gallery',
  

  components: {
    
  },

  data: () => ({
    //
  }),
};
</script>