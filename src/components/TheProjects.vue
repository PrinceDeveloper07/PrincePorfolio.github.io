<template>
  <v-container class="">
    <v-container>
      <v-row dense>
        <v-col
          v-for="(projects, index) in project"
          :key="index"
          cols="12"
          md="6"
          lg="6"
          xl="6"
        >
          <v-card class="mx-auto cards" max-width="400">
            <v-img
              class="white--text align-end"
              height="200px"
              :src="projects.img"
            >
            </v-img>

            <v-card-title class="teal--text">{{ projects.title }}</v-card-title>
            <v-card-text class="grey--text">
              <div>{{ projects.content }}</div>
            </v-card-text>

            <v-card-actions>
              <v-btn color="teal" text>
                View
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: "TheProjects",
  data() {
    return {
      project: [
        {
          color: "#385F73",
          title: "Netflix Clone",
          id: 1,
          img: "/images/netflix.webp",
          content: "Build from Nuxt Js.",
        },
        {
          color: "#385F73",
          title: "Instagram Clone",
          id: 2,
          img: "/images/Instagram.webp",
          content: "Build from Vue Js/Vuetify",
        },
        {
          color: "#385F73",
          title: "Todo App",
          id: 3,
          img: "/images/todo.webp",
          content: "Build from Vue Js.",
        },
        {
          color: "#546E7A",
          title: "FootMax",
          id: 4,
          img: "/images/addTocart.webp",
          content: "Simple add To cart. Build from Vue Js.",
        },
      ],
    };
  },
};
</script>
