<template>
  <div class="mt-16 ml-16">
    <div
      class="font-weight-bold text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4"
    >
      Programming Languages & tools
    </div>
    <div class="list-icons mt-5">
      <v-row>
        <v-icon x-large class="" color="blue-grey lighten-2">{{ html }}</v-icon>
        <v-icon x-large class="" color="blue-grey lighten-2">{{ css }}</v-icon>
        <v-icon x-large class="" color="blue-grey lighten-2"
          >mdi-language-javascript</v-icon
        >
        <v-icon x-large class="" color="blue-grey lighten-2">mdi-vuejs</v-icon>
        <v-icon x-large class="" color="blue-grey lighten-2">mdi-nuxt</v-icon>
        <v-icon x-large class="" color="blue-grey lighten-2"
          >mdi-bootstrap</v-icon
        >
        <v-icon x-large class="" color="blue-grey lighten-2"
          >mdi-vuetify</v-icon
        >
        <v-icon x-large class="" color="blue-grey lighten-2">mdi-sass</v-icon>
        <v-icon x-large class="" color="blue-grey lighten-2"
          >mdi-wordpress</v-icon
        >
      </v-row>
      <div class="mt-16">
        <div class="wrapper">
          <div v-for="item in items" :key="item.id">
            <span>
              <v-icon>{{ item.icon }}</v-icon>
            </span>
            <span class="text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4">{{
              item.title
            }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { mdiLanguageHtml5 } from "@mdi/js";
import { mdiLanguageCss3 } from "@mdi/js";

export default {
  name: "TheSkills",
  data() {
    return {
      html: mdiLanguageHtml5,
      css: mdiLanguageCss3,
      items: [
        { title: "Mobile-First, Responsive Design", icon: "mdi-check-bold" },
        { title: "Cross Browser Testing & Debugging", icon: "mdi-check-bold" },
        { title: "Cross Functional Teams", icon: "mdi-check-bold" },
        { title: "Agile Development & Scrum", icon: "mdi-check-bold" },
      ],
    };
  },
};
</script>
