<template>
    <div id = 'homepage'>
        <v-container>
                <v-layout column>
                    <v-carousel>
                        <v-carousel-item
                            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
                            cover
                        ></v-carousel-item>

                        <v-carousel-item
                            src="./../../public/kenny-eliason-1-aA2Fadydc-unsplash.jpg"
                            cover
                        ></v-carousel-item>

                        <v-carousel-item
                            src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                            cover
                        ></v-carousel-item>
                    </v-carousel>
                    </v-layout>
                    <v-layout>
                    <v-container>
                        <v-row align="center" justify="center">
                            <div class="d-flex align-center flex-column">
                                <v-card
                                width="400"
                                title="About Strath Kenya College"
                                text="Once upon a time, nestled within the vibrant heart of a bustling city, stood the humble beginnings of what would later flourish into a renowned institution of higher learning - Riverside University."
                                ></v-card>
                                <div class="mt-4 text-subtitle-2"></div>

                                <v-card width="400">

                                <template v-slot:title>
                                    The Journey
                                </template>

                                <template v-slot:subtitle>
                                    
                                </template>

                                <template v-slot:text>

                                    Founded in 1898 by a visionary group of educators and community leaders, Riverside University began as a small, local college with just a handful of students eager to pursue knowledge in an array of disciplines. Originally housed in a modest building on the outskirts of town, the university's mission was clear: to provide accessible and quality education to all who sought it, regardless of background or circumstance.

                                    Today, Riverside University stands as a beacon of knowledge, diversity, and innovation, its sprawling campus a testament to its rich history and enduring legacy. From its humble beginnings over a century ago to its present-day status as a world-class institution, Riverside University continues to inspire generations of students to pursue their dreams and make a positive impact on the world.
                                </template>
                                </v-card>

                                <div class="mt-4 text-subtitle-2"></div>

                                <v-card width="400">
                                <v-card-item>
                                    <v-card-title>Where we are</v-card-title>

                                </v-card-item>

                                <v-card-text>
                                    <p>
                                    As the years passed, Riverside University steadily expanded, fueled by a dedicated faculty, passionate students, and a commitment to academic excellence. With each passing decade, new programs were added, facilities were built, and the university's reputation grew.
                                    </p>
                                </v-card-text>
                                </v-card>
                            </div>
                        </v-row>
                    </v-container>
                </v-layout>
            </v-container>
    </div>
</template>
<script setup>
  const variants = ['elevated', 'flat', 'tonal', 'outlined']
</script>