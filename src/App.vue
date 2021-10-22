<template>
  <v-app>
    
     <Header /> 

    <v-main>
        <!-- Hero section  -->
        <HeroComponent />

        <!-- About us  -->
        <Aboutus />

        <!-- Protfolio -->
        <Protfolio />

        <!-- Project  -->
        <Project />

        <!-- Gallery  -->
        <Gallery />

        <!-- contactus  -->
        <Contactus />


        
    </v-main>
  </v-app>
</template>

<script>
import Aboutus from './components/Aboutus.vue';
import Contactus from './components/Contactus.vue';
import Gallery from './components/Gallery.vue';
// import HelloWorld from './components/HelloWorld';
import Header from './components/Header.vue';
import HeroComponent from './components/HeroComponent.vue';
import Project from './components/Project.vue';
import Protfolio from './components/Protfolio.vue';
export default {
  name: 'App',
  components: {
    Header,
    HeroComponent,
    Aboutus,
    Protfolio,
    Project,
    Gallery,
    Contactus
  },
  data() {
    return {
      menus: [
        {title:'Home' ,   route:'home'},
        {title:'Protfolio', route:'protfolio'},
        {title:'Project', route:'project'},
        {title:'Gallery', route:'gallery'},
        {title:'Service', route:'service'},
        {title:'Contact', route:'contact'},
      ]
    }
  }
};
</script>