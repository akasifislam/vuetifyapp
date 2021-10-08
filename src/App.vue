<template>
  <v-app>
    <v-app-bar
      app
      color="white"
      light
      elovation="6"
    >
    <v-toolbar-title>
      Vuetify App
    </v-toolbar-title>
    <v-spacer />
    <v-list class="d-flex align-center">
      <v-list-item link v-for="(menu,index) in menus" :key="index" :to="menu.route">
        <v-list-item-title> {{ menu.title }} </v-list-item-title>
      </v-list-item>
    </v-list>

    <v-btn>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>



    </v-app-bar>
    

    <v-main>
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
export default {
  name: 'App',
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