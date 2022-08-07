<template>
<NavBar/>
 <HeroSection/>
  <AboutComponent/>
 <ResumeComponent id="resume"/>
<PortFolio/>
<ContactComponent/>
<FooterSection/>
</template>

<script>
import NavBar from "./components/NavBar.vue"
import HeroSection from "./components/HeroSection.vue"
import AboutComponent from "./components/AboutComponent"
import ResumeComponent from "./components/ResumeComponent"
import PortFolio from "./components/PortFolio"
import ContactComponent from "./components/ContactComponent"
import FooterSection from "./components/FooterSection"
export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    AboutComponent,
    ResumeComponent,
    PortFolio,
    ContactComponent,
    FooterSection
   
   
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
