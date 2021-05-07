<template>
    <v-img :src="require('/src/assets/backgroundHud.png')" id="bg">
        <div id="cvbody" >
          <div id="video" data-aos="fade-right" data-aos-offset="300" data-aos-duration="1000">
              <iframe src="https://www.youtube.com/embed/LKnso2aqAq8" title="Video CV" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </div>
          <div id="socials">
              <a id="email" href="mailto:ines.piatkowska1@gmail.com" target="_blank">EMAIL</a>
              <a id="linkedin" href="https://www.linkedin.com/in/inespiatkowska/" target="_blank">LINKEDIN</a>
              <a id="instagram" href="https://www.instagram.com/ineesxx/" target="_blank">INSTAGRAM</a>
          </div>
        </div>
    </v-img>
</template>

<script>

  export default {
    name: 'VideoCv',

    components: {

    },

    data: () => ({
      
    }),

    methods: {

      },
    
  }
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@600&display=swap');

  template {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    
  }

  #cvbody{
      height: auto;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 50px;
      overflow-x: hidden;
  }
  #bg{
    width: 100vw;
    height: 100vh;
    display: fixed;

  }

    iframe {
      width: 375px; 
      height: 300px;
      margin-bottom: 40px;
    }

    #email, #linkedin, #instagram {
        text-decoration: none;
        color: #FFDD00;
        font-size: 16px;
        letter-spacing: 2px;
    }

    #email, #linkedin {
        margin-right: 50px;
    }

@media only screen and (min-width: 688px) {
  iframe {
      width: 688px; 
      height: 400px;
      margin-bottom: 40px;
    }

    #email, #linkedin, #instagram {
        text-decoration: none;
        color: #FFDD00;
        font-size: 18px;
        letter-spacing: 6px;
    }

    #email, #linkedin {
        margin-right: 50px;
    }
}

@media only screen and (min-width: 992px) {
  iframe {
      width: 850px; 
      height: 600px;
      margin-bottom: 40px;
    }

    #email, #linkedin, #instagram {
        text-decoration: none;
        color: #FFDD00;
        font-size: 18px;
        letter-spacing: 10px;
    }

    #email, #linkedin {
        margin-right: 50px;
    }
}

@media only screen and (min-width: 1312px) {
  #cvbody{
      height: auto;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 50px;
      overflow-x: hidden;
  }

    iframe {
      width: 958px; 
      height: 625px;
      margin-bottom: 40px;
    }

    #email, #linkedin, #instagram {
        text-decoration: none;
        color: #FFDD00;
        font-size: 20px;
        letter-spacing: 12px;
    }

    #email, #linkedin {
        margin-right: 220px;
    }
}

</style>