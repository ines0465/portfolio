<template>
  <div class="black" id="resumebody">
    <v-row id="resume">
      <h1 id="resumetitle">RESUME</h1>
    </v-row>
    <div id="resumepic">
        <a :href="resume" target="_blank">
            <v-img id="resumeimg" :src="require('/src/assets/resume.png')" />
        </a>
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

#resumebody {
  height: auto;
  width: 100vw;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  padding: 20px;

}
#resume{
  width: 100%;
  justify-content: center;
  margin-top: 40px;
}

#resumetitle{
  color: transparent;
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #FFDD00;
  font-size: 40px;
}

#resumepic {
    display: flex;
    justify-content: center;
    margin-top: 40px;
    margin-bottom: 40px;
}

#resumeimg {
    width: 300px;
    height: 400px;
}

@media only screen and (min-width: 688px) {
    #resumetitle{
    color: transparent;
    -webkit-text-stroke-width: 2px;
    -webkit-text-stroke-color: #FFDD00;
    font-size: 60px;
    }

    #resumeimg {
    width: 500px;
    height: 700px;
}
}

@media only screen and (min-width: 1312px) {
    #resumeimg {
    width: 600px;
    height: 900px;
    }
}
</style>

<script>

export default {
  name: 'Resume',
  

  components: {
    
  },

  data: () => ({
    resume: '../files/resume.png'
  }),
};
</script>