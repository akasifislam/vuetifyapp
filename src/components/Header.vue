<template>
  <v-app-bar
      app
      color="white"
      light
      elovation="6"
      elevate-on-scroll
    >
    <v-toolbar-title>
      Web Wild
    </v-toolbar-title>
    <v-spacer />
    <v-list class="d-flex align-center">
      <v-list-item link v-for="(menu,index) in menus" :key="index" :to="menu.route">
        <v-list-item-title> {{ menu.title }} </v-list-item-title>
      </v-list-item>
    </v-list>

    <v-btn text>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>
    <v-btn outlined color="success">Get Started</v-btn>



    </v-app-bar>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
export default {
  name: 'Header',
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
<style>
  .v-toolbar__title {
    font-size: 32px;
    color: rgba(230, 59, 59, 0.808);
    font-family: cursive;
    font-weight: 700;
    }
</style>