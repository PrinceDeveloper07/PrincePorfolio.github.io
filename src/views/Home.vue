<template>
<div>
  <Banner/>
  <AboutSection />
  <Skills />
  <TheProjects />
  <Footer />
</div>
</template>

<script>
import Banner from '../components/Banner'
import AboutSection from '../components/AboutSection'
import Skills from '../components/Skills'
import Footer from '../components/Footer'
import TheProjects from '../components/TheProjects'

export default {
  name: 'Home',
  components: {
    Banner,
    AboutSection,
    Skills,
    Footer,
    TheProjects
  }
}
</script>
<style lang="scss" scoped>

</style>
