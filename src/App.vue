<template>
  <v-app>
    
     <Header /> 

    <v-main>
        <!-- Hero section  -->
        <HeroComponent />
        <!-- About us  -->
        <Aboutus />
        <!-- Protfolio -->
        <Protfolio/>
    </v-main>
  </v-app>
</template>

<script>
import Aboutus from './components/Aboutus.vue';
// import HelloWorld from './components/HelloWorld';
import Header from './components/Header.vue';
import HeroComponent from './components/HeroComponent.vue';
import Protfolio from './components/Protfolio.vue';
export default {
  name: 'App',
  components: {
    Header,
    HeroComponent,
    Aboutus,
    Protfolio
  },
  data() {
    return {
      menus: [
        {title:'Home' ,   route:'home'},
        {title:'Profile', route:'profile'},
        {title:'Project', route:'project'},
        {title:'Service', route:'service'},
        {title:'Contact', route:'contact'},
      ]
    }
  }
};
</script>