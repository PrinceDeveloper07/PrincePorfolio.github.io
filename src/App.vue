<template>
  <v-app>
      <Navigation />
      <router-view></router-view>
    <v-main>
      
    </v-main>
  </v-app>
</template>

<script>
import Navigation from './components/Navigation'


export default {
  name: 'App',

  components: {
    Navigation,
  
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="scss" scoped>


</style>