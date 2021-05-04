<template>
  <div id="whole">
    <div id="main">
        </div>
        <div id="right" > 
        <v-img id="aboutmeimg"
        :src="require('../assets/portfoliopic.png')"></v-img>
        </div>
        <div class="text" id="aboutmetext" >
             <p>
             My name is Ines Piątkowska. I'm a graphic designer and an aspiring creative director. My main skills include creative/art. Direction, UX & UI design.
            I have experience in logo creation, web design, content creation and editing.
            I am always looking for new ways to showcase my style and creativity through design and film.
            </p>
    </div>
  </div>
</template>


<script>

  export default {
    name: 'AboutMe2',

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

  template {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
  }

  #whole{
      height: 235vh;
      background: #F2F2F2;
      display: flex;
      flex-direction: row;
  }

  #main{
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-direction: column;
      padding: 80px 2px;
  }

    #aboutmetitle{
        color: black;
        font-size: 5em;
        text-transform: lowercase;
        font-weight: normal;
        position: relative;
        transform: translateX(-5%);
    }

    #aboutmetext{
        max-width: 700px;
        font-size: 20px;
        padding: 10px;
        margin-bottom: 30px;
        margin-top: 300px;
    }

    #aboutmeimg {
      height: 300px;
      width: 300px;
      
    }

  @media only screen and (min-width: 403px){
    #whole{
      height: 210vh;
      background: #F2F2F2;
  }
  }

@media only screen and (min-width: 958px) {
  #aboutmetext{
        max-width: 958px;
        font-size: 20px;
        padding: 0;
        margin-bottom: 30px;
    }
}



@media only screen and (min-width: 1200px) {
  #whole{
      height: 240vh;
      background: #F2F2F2;
  }
  

}


@media only screen and (min-width: 1400px) {
  #whole{
      height: 220vh;
      background: #F2F2F2;
  }
}


</style>