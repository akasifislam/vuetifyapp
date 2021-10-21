<template>
  <v-app>
    
     <Header /> 

    <v-main>
        <!-- Hero section  -->
        <HeroComponent />
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
import Header from './components/Header.vue';
import HeroComponent from './components/HeroComponent.vue';
export default {
  name: 'App',
  components: {
    Header,
    HeroComponent
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