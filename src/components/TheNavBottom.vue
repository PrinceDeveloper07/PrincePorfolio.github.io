<template>
  <v-bottom-navigation
    :value="value"
    color="teal"
    grow
    app
    fixed
    dark
    height="50"
    class="hidden-xl-only hidden-lg-only"
  >
    <v-btn depressed route to="/">
      <v-icon>mdi-home</v-icon>
    </v-btn>

    <v-btn route to="/about">
      <v-icon>mdi-book</v-icon>
    </v-btn>

    <v-btn route to="/projects">
      <v-icon>mdi-web</v-icon>
    </v-btn>
    <v-btn route to="/skills">
      <v-icon>mdi-lightbulb</v-icon>
    </v-btn>
    <v-btn>
      <v-switch
        :value="darkMode"
        @change="toggleDarkMode"
        :label="` ${switchLabel} `"
      ></v-switch>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
export default {
  name: "TheNavBottom",
  data: () => ({
    value: 1,
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
