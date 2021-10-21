<template>
    <v-container>
        <v-row>
            <v-col lg="6">
                <h2>Welcome to Our Vuetify App</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum necessitatibus repudiandae porro atque praesentium assumenda nulla earum sit quibusdam cupiditate?
                </p>
                <v-btn color="success" class="white--text" rounded>Get Started</v-btn>
                <v-btn color="indigo" class="white--text" rounded>
                    <v-icon>mdi-play-circle</v-icon>
                    Watch video
                </v-btn>
            </v-col>
            <v-col lg="6">
                <img width="100%" src="./../assets/hero-image.jpg" alt="">
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: "HeroComponent"
}
</script>

<style>

</style>