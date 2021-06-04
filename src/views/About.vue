<template>
<div>
  <Discover />
    <div>
      <v-container class="" id="discover-page">
        <v-row class="d-flex justify-center align-center">
          <v-col
          cols="3"
          md="4">
            <v-img
              class="circle-img"
              max-height="250"
              max-width="250"  
              src="../assets/profile-2.jpg"
              >
            </v-img>
          </v-col>
          <v-col
            cols="8"
            md="7">
            <div>
                <h1 class="orange--text display-2">Front-End Developer</h1>
                <span class="purple--text display-1">Christian Prince</span>
            </div>
            <div>
                <p>Hi! I am Christian Prince, a web designer/developer focused on crafting great web experiences. Designing and Coding have been my passion since the days I started working with computers but I found myself into web design/development since 2019. I enjoy creating beautifully designed, intuitive and functional websites.
                  </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <Footer />
</div>
</template>

<script>
import Discover from '../components/Discover'
import Footer from '../components/Footer'

export default {
  name: 'about',
  components: {
    Discover,
    Footer
  }
}
</script>
<style lang="scss" scoped>

#discover-page{
  height: 500px;
  margin-top: 150px;




  .circle-img{
    border-top-left-radius: 100% 100%;
    border-top-right-radius: 100% 100%;
    border-bottom-right-radius: 100% 100%;
    border-bottom-left-radius: 100% 100%;
    padding: 5rem;
  }
}

</style>


