<template>
  <v-app class="app">
    <TheNavigationDrawer />
    <v-main>
      <router-view></router-view>
    </v-main>

    <v-footer padless>
      <TheNavBottom />
    </v-footer>
  </v-app>
</template>

<script>
import TheNavigationDrawer from "./components/TheNavigationDrawer.vue";
import TheNavBottom from "./components/TheNavBottom.vue";

export default {
  name: "App",
  components: {
    TheNavigationDrawer,
    TheNavBottom,
  },
};
</script>

<style lang="scss" scoped></style>
