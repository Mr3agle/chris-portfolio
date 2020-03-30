<template>
  <div>
    <v-container>
      <v-row dense>
        <v-col cols="12">
          <v-card color="white" light elevation="5">
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar class="ma-3" size="225" tile>
                <v-img src="/img/games/witch1.png"></v-img>
              </v-avatar>
              <div>
                <v-card-title class="display-2">The Witch</v-card-title>

                <v-card-subtitle
                  class="mt-1 subtitle-1"
                >The Witch es una experiencia de horror, en la cual el usuario deberá pasar una noche un aterrador bosque y descubrir lo que acecha en la oscuridad.</v-card-subtitle>
                <v-card-subtitle>El juego fue desarrollado en Unity y programado en CSharp para Gear VR. La mayoría de assets son externos y de uso libre con algunos creados por mí.</v-card-subtitle>
              </div>
            </div>
          </v-card>
        </v-col>
      </v-row>
      <v-row class="my-10">
        <v-col>
          <v-card elevation="5">
            <v-card-title class="display-1 text-center">Videos</v-card-title>
            <v-row>
              <v-col>
                <video class="px-3" src="/video/The witch trailer.mp4" width="100%" controls></video>
              </v-col>
              <v-col>
                <video class="px-3" src="/video/witchGameplay.mp4" width="100%" controls></video>
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <v-card elevation="5">
            <v-card-title class="display-1 text-center">Screenshots</v-card-title>
            <v-row>
              <v-carousel class="my-5 px-7" hide-delimiters>
                <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src"></v-carousel-item>
              </v-carousel>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
      <v-row class="mt-7">
        <v-col>
          <v-hover>
            <template v-slot:default="{ hover }">
              <v-card class="mx-auto" max-width="300">
                <v-img src="/img/games/apebash (1).png">
                  <v-card-text>
                    <h2 class="title white--text">Ape Bash</h2>
                  </v-card-text>
                </v-img>

                <v-fade-transition>
                  <v-overlay v-if="hover" absolute color="white">
                    <v-btn to="/apebash">
                      <v-icon>mdi-chevron-left</v-icon>
                    </v-btn>
                  </v-overlay>
                </v-fade-transition>
              </v-card>
            </template>
          </v-hover>
        </v-col>
        <v-col>
          <v-hover>
            <template v-slot:default="{ hover }">
              <v-card class="mx-auto" max-width="300">
                <v-img src="/img/games/majini/majini (1).png">
                  <v-card-text>
                    <h2 class="title white--text">Majini</h2>
                  </v-card-text>
                </v-img>

                <v-fade-transition>
                  <v-overlay v-if="hover" absolute color="white">
                    <v-btn to="/majini">
                      <v-icon>mdi-chevron-right</v-icon>
                    </v-btn>
                  </v-overlay>
                </v-fade-transition>
              </v-card>
            </template>
          </v-hover>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: '/img/games/witch1.png',
        },
        {
          src: '/img/games/witch2.png',
        },
        {
          src: '/img/games/witch3.png',
        }
      ]
    }
  },
}
</script>