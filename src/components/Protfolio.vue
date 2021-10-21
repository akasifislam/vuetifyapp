<template>
  <v-container class="my-15">
      <v-row justify="center">
          <v-col lg="12" class="text-center">
              <v-subheader class="text-h4 justify-center">Protfolio</v-subheader>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cumque, a officiis. Placeat corrupti atque nobis?</p>
          </v-col>
          <v-col lg="12">
              <div class="text-center">
                  <v-chip @click="activeProtfolio='webapp'" :color="activeProtfolio === 'webapp' ? 'success':'' " class="mx-2">Web App</v-chip>
                  <v-chip @click="activeProtfolio='mobileapp'" :color="activeProtfolio === 'mobileapp' ? 'success':'' " class="mx-2">Mobile App</v-chip>
                  <v-chip @click="activeProtfolio='desktopapp'" :color="activeProtfolio === 'desktopapp' ? 'success':'' " class="mx-2">Desktop App</v-chip>
              </div>
          </v-col>
          <v-col lg="3" v-for="(web,webindex) in webApps" :key="webindex">
            <v-img
              :src="web.image"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
            >
              <v-card-title> {{ web.title }} </v-card-title>
            </v-img>
            <v-card>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Temporibus fugiat, placeat tempore eveniet ea exercitationem earum assumenda amet non iste sequi tempora sunt quidem reprehenderit doloribus qui, in perferendis ratione!
            </v-card>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
export default {
    data() {
        return {
            activeProtfolio: 'webapp',
            webApps:[
                {title:'Web Application',image:''},
                {title:'Mobile Application',image:''},
                {title:'Desktop Application',image:''}
            ]
        }
    }
}
</script>

<style>

</style>