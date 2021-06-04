<template>
    <v-container fluid  id="banner" class="d-flex align-center justify-center">
      <div class="">
        <div class="content">
              <h1 class="white--text  display-2 text-center mb-5">Christian Prince</h1>
              <p class="white--text font-weight-small display-4 text-center">Front-End Developer</p>
              <div class="text-center">
                <a download href="/files/resumei.pdf" style="text-decoration: none;">
                  <v-btn  rounded class="purple white--text">Download Resumei</v-btn>
                </a>
              </div>
        </div>
        <!-- <div>
          <h1 class="white--text font-weight-bold display-2">&lt;Coder&gt;</h1>
          <p class="white--text font-weight-small display-1">Front-end Developer<span><br>who is focusing in clean <br>code.</span></p>
        </div> -->
      </div>
    </v-container>
</template>

<script>

export default {
  data: () =>({
    
    
    
  }),
  methods: {
            download () {
                const url = '../assets/CV-RESUMEI.PDF';
                window.location.href = url;
            }
        },
    
}
</script>

<style lang="scss" scoped>
#banner{
  background-image:
	linear-gradient(to bottom right,#ef890ad4 40%,#fb8c00d4  75%),
  url(../assets/background.jpg);
	background-position: center;
	background-size: cover;
  background-attachment: fixed;
  background-repeat: no-repeat;
	min-height: 600px;
}



</style>