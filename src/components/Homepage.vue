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
                                <div class="text-subtitle-2">With props</div>

                                <v-card
                                width="400"
                                title="This is a title"
                                subtitle="This is a subtitle"
                                text="This is content"
                                ></v-card>

                                <div class="mt-4 text-subtitle-2">With slots</div>

                                <v-card width="400">
                                <template v-slot:title>
                                    This is a title
                                </template>

                                <template v-slot:subtitle>
                                    
                                </template>

                                <template v-slot:text>
                                    Once upon a time, nestled within the vibrant heart of a bustling city, stood the humble beginnings of what would later flourish into a renowned institution of higher learning - Riverside University.

                                    Founded in 1898 by a visionary group of educators and community leaders, Riverside University began as a small, local college with just a handful of students eager to pursue knowledge in an array of disciplines. Originally housed in a modest building on the outskirts of town, the university's mission was clear: to provide accessible and quality education to all who sought it, regardless of background or circumstance.

                                    As the years passed, Riverside University steadily expanded, fueled by a dedicated faculty, passionate students, and a commitment to academic excellence. With each passing decade, new programs were added, facilities were built, and the university's reputation grew.

                                    During the tumultuous years of the mid-20th century, Riverside University played a vital role in shaping the cultural and intellectual landscape of its community. It became a hub for innovation and social progress, fostering dialogue and debate on pressing issues of the time.

                                    In the latter half of the century, Riverside University solidified its standing as a leading research institution, attracting scholars and researchers from around the globe. Breakthroughs in science, technology, and the arts emanated from its laboratories and lecture halls, leaving an indelible mark on the world.

                                    As the new millennium dawned, Riverside University embraced the digital age, leveraging technology to enhance learning and expand its reach beyond physical boundaries. Online courses, virtual libraries, and collaborative research projects became integral parts of the university experience.

                                    Today, Riverside University stands as a beacon of knowledge, diversity, and innovation, its sprawling campus a testament to its rich history and enduring legacy. From its humble beginnings over a century ago to its present-day status as a world-class institution, Riverside University continues to inspire generations of students to pursue their dreams and make a positive impact on the world.
                                </template>
                                </v-card>

                                <div class="mt-4 text-subtitle-2">With markup</div>

                                <v-card width="400">
                                <v-card-item>
                                    <v-card-title>This is a title</v-card-title>

                                    <v-card-subtitle>This is a subtitle</v-card-subtitle>
                                </v-card-item>

                                <v-card-text>
                                    This is content
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