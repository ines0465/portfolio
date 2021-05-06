<template>
  <div id="whole" class="black" >
        <div id="right" > 
        <v-img id="aboutmeimg"
        :src="require('../assets/picportfolio.png')"></v-img>
        </div>
        <div class="text" id="aboutmetext" >
             <h1 id="bigtext">HI THERE!</h1>
             <p id="smalltext1">
             My name is Ines Piątkowska. I'm a graphic designer and an aspiring creative director. My main skills include creative/art. Direction, UX & UI design.
             </p>
            <p id="smalltext2">I have experience in logo creation, web design, content creation and editing.
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
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@600&display=swap');

  template {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    background-color: black;
    
  }

  #whole{
      height: auto;
      display: flex;
      flex-direction: column-reverse;
      background: black;
      align-items: center;
      justify-content: space-around;
      overflow-x: hidden;

  }

    #bigtext{
        max-width: 700px;
        font-size: 40px;
        padding: 40px;
        margin-bottom: 10px;
        color: white;
        letter-spacing: 20px;
    }

    #smalltext1{
        max-width: 600px;
        font-size: 16px;
        padding: 40px;
        margin-bottom: 10px;
        margin-top: 0px;
        color: white;
        font-family: 'Raleway', sans-serif;
        font-weight: 600;
    }

    #smalltext2{
      max-width: 600px;
      font-size: 16px;
      padding: 40px;
      margin-top: 0px;
      color: white;
      font-family: 'Raleway', sans-serif;
      font-weight: 600;
    }

    #aboutmeimg {
      height: 300px;
      width: 200px;
    }

  @media only screen and (min-width: 992px){
    #whole{
      height: auto;
      display: flex;
      flex-direction: row;
      background: black;
      align-items: center;
      justify-content: space-around;

  }

    #bigtext{
        max-width: 700px;
        font-size: 50px;
        padding: 40px;
        margin-bottom: 10px;
        color: white;
        letter-spacing: 20px;
    }

    #smalltext1{
        max-width: 600px;
        font-size: 18px;
        padding: 40px;
        margin-bottom: 10px;
        margin-top: 0px;
        color: white;
        font-family: 'Raleway', sans-serif;
        font-weight: 600;
    }

    #smalltext2{
      max-width: 600px;
      font-size: 18px;
      padding: 40px;
      margin-top: 0px;
      color: white;
      font-family: 'Raleway', sans-serif;
      font-weight: 600;
    }

    #aboutmeimg {
      height: 300px;
      width: 200px;
    }
  }

  @media only screen and (min-width: 1312px){
    #whole{
      height: auto;
      display: flex;
      flex-direction: row;
      background: black;
      align-items: center;
      justify-content: space-around;

  }

    #bigtext{
        max-width: 700px;
        font-size: 60px;
        padding: 40px;
        margin-bottom: 10px;
        color: white;
        letter-spacing: 20px;
    }

    #smalltext1{
        max-width: 600px;
        font-size: 20px;
        padding: 40px;
        margin-bottom: 10px;
        margin-top: 0px;
        color: white;
        font-family: 'Raleway', sans-serif;
        font-weight: 600;
    }

    #smalltext2{
      max-width: 600px;
      font-size: 20px;
      padding: 40px;
      margin-top: 0px;
      color: white;
      font-family: 'Raleway', sans-serif;
      font-weight: 600;
    }

    #aboutmeimg {
      height: 500px;
      width: 350px;
    }
  }
</style>