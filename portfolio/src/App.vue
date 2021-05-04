<template>
  <v-app>
    <NavBar />
    <AboutMe />
    <AboutMe2 />
  </v-app>
</template>

<script>


export default {
  name: 'App',

  components: {
    NavBar: () => import('@/components/NavBar'),
    AboutMe: () => import('@/components/AboutMe'),
    AboutMe2: () => import('@/components/AboutMe2'),
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="scss">
 html {
  scroll-behavior: smooth;
}
</style>