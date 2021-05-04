<template>
  <div>
    <v-app-bar
      color="black"
      dark
    >
      
      <v-toolbar-title class="font-weight-bold">portfolio</v-toolbar-title>

      <v-spacer></v-spacer>

    <div id="links">

      <v-btn
      text
      color="white"
      class="text-lowercase"
      >
        <a id="navigationbutton" href="#whole">ABOUT ME</a>
        
      </v-btn>

      <v-btn
      text
      color="white"
      class="text-lowercase">
      <a id="navigationbutton" href="#servicebody">
        WORK
        </a>
      </v-btn>

      <v-btn
      text
      color="white"
      class="text-lowercase">
        <a id="navigationbutton" href="#skillsbody">RESUME</a>
      </v-btn>
    </div>
    <v-app-bar-nav-icon @click="drawer = true"
    id="burger" ></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      color="black"
      
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          
        >
          <v-list-item>
            <v-list-item-title class="white--text" id="burgerbuttons"><a id="navigationbutton" href="#whole">ABOUT ME</a></v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title class="white--text" id="burgerbuttons"><a id="navigationbutton" href="#servicebody">WORK</a></v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title class="white--text" id="burgerbuttons"><a id="navigationbutton" href="#skillsbody">RESUME</a></v-list-item-title>
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
  }

  #navigationbutton{
    text-decoration: none;
    color: white;
  }

  @media only screen and (min-width: 749px) {
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