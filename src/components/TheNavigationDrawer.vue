<template>
  <div class="hidden-xs-only">
    <v-navigation-drawer flat width="300" app class="teal lighten-1">
      <div class="d-flex justify-center align-center flex-column mt-16">
        <v-img
          class="circle-img"
          width="100"
          src="/images/profile.webp"
        ></v-img>
        <v-row class="mt-2">
          <v-icon class="mr-1" color="white">mdi-facebook</v-icon>
          <v-icon class="mr-1" color="white">mdi-instagram</v-icon>
          <v-icon class="mr-1" color="white">mdi-github</v-icon>
          <v-icon color="white">mdi-linkedin</v-icon>
        </v-row>
      </div>
      <v-list dense nav flat class="mt-16">
        <v-list-item
          v-for="link in links"
          :key="link.title"
          class="ml-5 ma-0 text-center"
          route
          :to="link.route"
          replace
        >
          <v-list-item-content>
            <v-list-item-title class="font-weight-light white--text">{{
              link.text
            }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar flat app>
      <v-switch
        :value="darkMode"
        @change="toggleDarkMode"
        :label="` ${switchLabel} `"
      ></v-switch>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: "TheNavigationDrawer",
  data: () => ({
    darkMode: false,
    links: [
      {
        id: 1,
        text: "Home",
        icon: "mdi-view-dashboard",
        route: "/",
      },
      {
        id: 2,
        text: "Discover",
        icon: "mdi-account",
        route: "/about",
      },
      {
        id: 3,
        text: "Projects",
        icon: "mdi-view-dashboard",
        route: "/projects",
      },
      {
        id: 4,
        text: "Skills",
        icon: "mdi-view-dashboard",
        route: "/skills",
      },
    ],
  }),
  methods: {
    toggleDarkMode: function() {
      this.$vuetify.theme.dark = !this.$vuetify.theme.dark;
      this.darkMode = !this.darkMode;
    },
  },
  computed: {
    switchLabel: function() {
      return this.darkMode ? "" : "";
    },
  },
};
</script>

<style lang="scss" scoped>
.circle-img {
  border-top-left-radius: 100% 100%;
  border-top-right-radius: 100% 100%;
  border-bottom-right-radius: 100% 100%;
  border-bottom-left-radius: 100% 100%;
  padding: 5rem;
}
</style>