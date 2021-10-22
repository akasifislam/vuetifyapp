<template>
    <v-footer
        dark
        padless
    >
        <v-card
        flat
        tile
        class="blue-grey darken-4 lighten-1 white--text text-center"
        >
        <v-card-text>
            <v-btn
            v-for="icon in icons"
            :key="icon"
            class="mx-4 white--text"
            icon
            >
            <v-icon size="24px">
                {{ icon }}
            </v-icon>
            </v-btn>
        </v-card-text>

        <v-card-text class="white--text pt-0">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quam non nostrum facere? Quas minima consequuntur vel pariatur corporis. Corporis expedita fuga voluptas iusto perspiciatis dolores laborum tempore. Esse laboriosam eum veniam dolor iure commodi. Laborum molestias esse nemo ipsam! Reprehenderit amet porro nulla facere ad!
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
            {{ new Date().getFullYear() }} — <strong>Web Wild</strong>
        </v-card-text>
        </v-card>
    </v-footer>
</template>

<script>
export default {

}
</script>

<style>

</style>