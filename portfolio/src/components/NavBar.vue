<template>
  <div>
    <v-app-bar
      color="#151415"
      dark
    >
      
      <v-toolbar-title>
        <img src="../assets/hud_circle.png" height="80" alt="">
      </v-toolbar-title>

      <v-spacer></v-spacer>

    <div id="links">

      <v-btn
      text
      color="white"
      class="text-uppercase"
      >
        <a id="navigationbutton" href="#whole">ABOUT ME</a>
        
      </v-btn>

      <v-btn
      text
      color="white"
      class="text-uppercase">
      <a id="navigationbutton" href="#gallery">
        WORK
        </a>
      </v-btn>

      <v-btn
      text
      color="white"
      class="text-uppercase">
        <a id="navigationbutton" href="#resume">RESUME</a>
      </v-btn>
    </div>
    <v-app-bar-nav-icon @click="drawer = true"
    id="burger" ></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      color="#151415"
      width="100%"
      
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          
        >
          <v-list-item @click="drawer = false">
            <v-list-item-title class="white--text" id="burgerbuttons"><a id="navigationbutton" href="#whole">ABOUT ME</a></v-list-item-title>
          </v-list-item>

          <v-list-item @click="drawer = false">
            <v-list-item-title class="white--text" id="burgerbuttons"><a id="navigationbutton" href="#gallery">WORK</a></v-list-item-title>
          </v-list-item>

          <v-list-item @click="drawer = false">
            <v-list-item-title class="white--text" id="burgerbuttons"><a id="navigationbutton" href="#resume">RESUME</a></v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500&display=swap');

  template {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    font-weight: 500;
  }

  #links{
    display: none;
  }

  #burgerbuttons {
    font-size: 2em;
    margin: 25px;
    padding: 10px;
    color: #FFDD00;
  }

  #navigationbutton{
    text-decoration: none;
    color: #FFDD00;
  }

  @media only screen and (min-width: 992px) {
    #burger {
      display: none;
    }
    #links {
      display: flex;
    }
  }

 </style>

  <script>
  export default {
    name: 'NavBar',

    components: {
      
    },

    data: () => ({
      drawer: false,
      group: null,
    }),

    methods: {

      },
    
  }
</script>