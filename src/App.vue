<template>
<NavBar/>
 <HeroSection/>
  <AboutComponent/>
 <ResumeComponent/>

</template>

<script>
import NavBar from "./components/NavBar.vue"
import HeroSection from "./components/HeroSection.vue"
import AboutComponent from "./components/AboutComponent"
import ResumeComponent from "./components/ResumeComponent"

export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    AboutComponent,
    ResumeComponent,
   
   
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
