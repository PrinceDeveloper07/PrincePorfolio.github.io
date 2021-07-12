<template>
  <v-container class="about">
    <TheAbout />
  </v-container>
</template>

<script>
import TheAbout from "../components/TheAbout";

export default {
  name: "about",
  components: {
    TheAbout,
  },
  data: () => ({
    items: [
      {
        icon: "mdi-plus-thick",
        text: "Inbox",
      },
      {
        icon: "mdi-plus-thick",
        text: "Star",
      },
      {
        icon: "mdi-plus-thick",
        text: "Send",
      },
      {
        icon: "mdi-plus-thick",
        text: "Drafts",
      },
    ],
    model: 1,
  }),
};
</script>