<template>
  <v-card max-width="100%" class="mx-auto" flat>
    <v-container>
      <v-row dense>
        <v-col v-for="(item, i) in items" :key="i" cols="12">
          <v-hover>
            <template v-slot:default="{ hover }">
              <v-card class="mx-auto my-5" :color="item.color" dark elevation="15">
                <v-img
                  :src="item.src"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="300px"
                >
                  <v-card-title class="headline" v-text="item.title"></v-card-title>

                  <v-card-subtitle v-text="item.description"></v-card-subtitle>
                </v-img>

                <v-fade-transition>
                  <v-overlay v-if="hover" absolute color="white">
                    <v-btn class="white" light :to="item.to">Ver Proyecto</v-btn>
                  </v-overlay>
                </v-fade-transition>
              </v-card>
            </template>
          </v-hover>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    overlay: false,
    items: [
      {
        color: '#1F7087',
        src: '/img/games/apebash (3).png',
        title: 'ApeBash',
        description: 'El juego fue desarrollado en Unity y programado en CSharp. La mayoría de assets son externos y de uso libre con algunos creados por mí. ',
        to: '/apebash'
      },
      {
        color: '#952175',
        src: '/img/games/majini/majini (1).png',
        title: 'Majini',
        description: 'El juego fue desarrollado en Unity y programado en CSharp para Gear VR. La mayoría de assets son externos y de uso libre con algunos creados por mí.',
        to: '/apebash'
      },
      {
        color: '#952175',
        src: '/img/games/witch1.png',
        title: 'The Witch',
        description: 'El juego fue desarrollado en Unity y programado en CSharp para Gear VR. La mayoría de assets son externos y de uso libre con algunos creados por mí.',
        to: '/apebash'
      }
    ],
  }),
}
</script>