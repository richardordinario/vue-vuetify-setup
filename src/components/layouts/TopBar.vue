<template>
    <section>
        <v-container>
            <v-layout justify-center>
                <v-flex xs12 md10 xl8>
                    <v-app-bar color="transparent" elevation="0" height="100">
                        <v-toolbar-title>
                            <v-img max-height="50" max-width="50" :src="require('../../assets/logo.png')"></v-img>
                        </v-toolbar-title>
                        <v-toolbar-items :class="$vuetify.breakpoint.smAndDown ? 'ml-5': ($vuetify.breakpoint.xl ? 'ml-16' : 'ml-12')">
                            <v-btn elevation="0" color="transparent" :class="$vuetify.breakpoint.smAndDown ? '': ($vuetify.breakpoint.xl ? 'mx-7' : 'mx-4')" :small="$vuetify.breakpoint.smAndDown">About</v-btn>
                            <v-btn elevation="0" color="transparent" :class="$vuetify.breakpoint.smAndDown ? '': ($vuetify.breakpoint.xl ? 'mx-7' : 'mx-4')" :small="$vuetify.breakpoint.smAndDown">Projects</v-btn>
                            <v-btn elevation="0" color="transparent" :class="$vuetify.breakpoint.smAndDown ? '': ($vuetify.breakpoint.xl ? 'mx-7' : 'mx-4')" :small="$vuetify.breakpoint.smAndDown">Contact</v-btn>
                        </v-toolbar-items>
                    </v-app-bar>
                </v-flex>
            </v-layout>
        </v-container>
    </section>
</template>

<script>
    export default {
        
    }
</script>