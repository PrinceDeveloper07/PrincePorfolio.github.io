<template>
  <div class="mx-16">
    <div class="mt-2 d-flex justify-center">
      <div>
        <v-img :src="img" width="300"></v-img>
      </div>
    </div>
    <div class="wrapper">
      <div
        class="font-weight-bold text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4"
      >
        How are you?
      </div>
      <p
        class="font-weight-light text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4"
      >
        I'm a <span class="teal--text">{{subTitle}}</span> focused on
        functionalities of great web experiences. Designing and Coding have been
        my passion since the days I started working with computers but I found
        myself into web design/development since 2019.
      </p>
    </div>
    <div class="education mt-16">
      <div>
        <div
          class="sub-title text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4 font-weight-bold"
        >
          Education
        </div>
        <div
          class="font-weight-light text-sm-body-2 text-md-body-1 text-lg-h6 text-xl-h4"
        >
          I took a course of Bachelor Science of Information Technology in AMA
          College. I start coding from college. There's a lot of field in IT,
          but I found my self into Web development
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheAbout",
  data() {
    return {
      subTitle: "Front-End Developer",
      img: "/images/website-build.svg",
    };
  },
};
</script>
