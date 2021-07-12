<template>
  <v-container class="main mt-16 ">
    <div class="" id="content">
      <div class="mx-16">
        <div>
          <p
            class="font-weight-bold mt-10 text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4"
            color="#455A64"
          >
            Hello There! I am Prince
          </p>
          <p class="font-weight-bold teal--text text-h4">Front-end Developer</p>
          <p class=" text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4">
            I am experienced in leveraging agile frameworks to provide a robust
            synopsis for high level overviews. Iterative approaches to corporate
            strategy foster collaborative thinking to further the overall value
            proposition.
          </p>
        </div>
      </div>
    </div>
  </v-container>
</template>
<script>
import { mdiLanguageHtml5 } from "@mdi/js";
import { mdiLanguageCss3 } from "@mdi/js";
import { mdiSass } from "@mdi/js";

export default {
  name: "TheHome",
  components: {},
  data() {
    return {
      html: mdiLanguageHtml5,
      css: mdiLanguageCss3,
      sass: mdiSass,
    };
  },
};
</script>

<style lang="scss" scoped>
.main {
  #content {
    p {
      font-size: 20px;
    }
    .circle-img {
      border-top-left-radius: 100% 100%;
      border-top-right-radius: 100% 100%;
      border-bottom-right-radius: 100% 100%;
      border-bottom-left-radius: 100% 100%;
      padding: 5rem;
    }
  }
}

@media screen and(min-width: 1920px) {
  #content {
    margin-top: 200px;
  }
}
</style>
