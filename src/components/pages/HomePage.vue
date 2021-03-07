<template>
    <section>
        <v-img max-height="900" :src="$vuetify.breakpoint.xs ? require('../../assets/mobile.png') : require('../../assets/hero.png')" dark>
            <TopBar/>
            <v-container>
                <v-layout justify-center>
                    <v-flex xs12 md11 xl8>
                        <v-row justify="center" :class="$vuetify.breakpoint.smAndDown ? 'my-5':'my-16'">
                            <v-col cols="12" md="6" sm="8">
                                <v-card elevation="0" color="transparent" max-width="500" class="mx-auto">
                                    <v-card-text>
                                        <div class="description mb-2 ml-1">Hi I am</div>
                                        <div class="name mb-5">Richard Ordinario</div>
                                        <v-btn outlined class="mb-5">WEB DEVELOPER</v-btn>
                                        <p class="description">I’m an all around web developer and have a good 
                                        knowledge in front and back end techniques. <br> <br> I love spending time on fixing little details and 
                                        optimizing web apps. Also i like working and 
                                        collaborating in a team not only to learn but also 
                                        to share my knowledge.
                                        </p>
                                        <br><br>
                                        <p class="description">Tech Stack</p>
                                        <v-img :src="require('../../assets/tech.png')" max-height="110" max-width="200"></v-img>
                                    </v-card-text>
                                </v-card>                            
                            </v-col>
                            <v-col cols="12" md="6" sm="4"></v-col>
                        </v-row>
                    </v-flex>
                </v-layout>
            </v-container>
        </v-img>
        <Projects/>
    </section>
</template>

<script>
import TopBar from '../layouts/TopBar'
import Projects from '../layouts/Projects'
export default {
    components: {
        TopBar,
        Projects
    }
}
</script>