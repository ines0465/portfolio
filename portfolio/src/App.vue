<template>
  <v-app id="app">
    <NavBar />
    <div id="banner">
      <p id="ines"> INESPIATKOWSKA</p>
      <p id="ines"> INESPIATKOWSKA</p>
      <p id="ines"> INESPIATKOWSKA</p>
    </div>
    <AboutMe />
    <AboutMe2 />
    <VideoCv /> 
    <Gallery />
    <Resume />
    <v-btn
            v-scroll="onScroll"
            v-show="fab"
            fab
            dark
            fixed
            bottom
            right
            color="transparent"
            @click="toTop"
            id="totopbutton"
          >
            <v-img :src="require('./assets/hud_circle.png')" height="80" width="80"></v-img>
          </v-btn>
  </v-app>
</template>

<script>


export default {
  name: 'App',

  components: {
    NavBar: () => import('@/components/NavBar'),
    AboutMe: () => import('@/components/AboutMe'),
    AboutMe2: () => import('@/components/AboutMe2'),
    VideoCv: () => import('@/components/CvVideo'),
    Gallery: () => import('@/components/Gallery'),
    Resume: () => import('@/components/Resume'),
  },

  data: () => ({
    fab: false,

  }),

  methods: {
    onScroll (e) {
      if (typeof window === 'undefined') return
      const top = window.pageYOffset ||   e.target.scrollTop || 0
      this.fab = top > 80
    },
    toTop () {
      this.$vuetify.goTo(0)
    }
  }
};
</script>

<style>
 html {
  scroll-behavior: smooth;
  
}

#totopbutton{
    z-index: 111;
    margin-right: 5vw;
}

#banner {
  display: none;
}

@media only screen and (min-width: 992px) {

  #banner{
    height: 100vh;
    width: 100px;
    position: fixed;
    right: 0;
    margin-top: 0.5vh;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-content: center;
    z-index: 999999;

  }
  #ines{
    color:#FFDD00;
    letter-spacing: 0.5vw;  
    transform: rotate(-270deg);
    -webkit-transform: rotate(-270deg);
    /* Firefox */
    -moz-transform: rotate(-270deg);

    /* IE */
    -ms-transform: rotate(-270deg);

    /* Opera */
    -o-transform: rotate(-270deg);

    /* Internet Explorer */
    filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);

  }
}

</style>