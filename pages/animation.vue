<template>
  <div>
    <v-row class="ml-1 mt-5">
      <div class="display-2">Sketches y Diseño de Personajes</div>
      <p
        class="mt-3"
      >Estos sketches fueron creados con l intención de dar vida a diferentes personajes, además de verlos en diferentes situaciones. Es el primer paso en el proceso de animación.</p>
    </v-row>
    <v-carousel class="my-5" hide-delimiters>
      <v-carousel-item v-for="(item,i) in sketches" :key="i" :src="item.src"></v-carousel-item>
    </v-carousel>

    <v-divider class="my-12" />

    <v-row class="ml-1 mt-5">
      <div class="display-2">Pruebas de Lápiz</div>
      <p
        class="mt-3"
      >Estas son animaciones simples para probar varios conceptos o movimientos antes de integrarlos a una animación final. Es el segundo paso en el proceso de animación.</p>
    </v-row>
    <v-carousel class="my-5" hide-delimiters>
      <v-carousel-item v-for="(item,i) in handraws" :key="i">
        <v-row justify="center">
          <video :src="item.src" controls></video>
        </v-row>
      </v-carousel-item>
    </v-carousel>

    <v-divider class="my-12" />

    <v-row class="ml-1 mt-5">
      <div class="display-2">Animación a Blanco y Negro</div>
      <p
        class="mt-3"
      >Animaciones casi finales, donde se asegura que las animaciones y concepto funcionen bien en conjunto antes de darles color. Es el tercer paso en el proceso de animación.</p>
    </v-row>
    <v-carousel class="my-5" hide-delimiters>
      <v-carousel-item v-for="(item,i) in bw" :key="i">
        <v-row justify="center">
          <video :src="item.src" controls height="500px"></video>
        </v-row>
      </v-carousel-item>
    </v-carousel>

    <v-divider class="my-12" />

    <v-row class="ml-1 mt-5">
      <div class="display-2">Producto Final</div>
      <p
        class="mt-3"
      >Animación llamada CHEESE que cuenta una historia de acerca de la discriminación, aquí vemos todos los procesos de animación trabajar en conjunto.</p>
    </v-row>
    <v-row justify="center">
      <video class="mt-5" src="/video/cheeseMockUp.mp4" controls height="500px"></video>
    </v-row>
  </div>
</template>


<script>
export default {
  data() {
    return {
      sketches: [
        {
          src: '/img/sketch1.png',
        },
        {
          src: '/img/sketch2.png',
        },
        {
          src: '/img/sketch3.png',
        },
        {
          src: '/img/sketch4.png',
        },
      ],
      handraws: [
        {
          src: '/video/ballMan1.mov',
        },
        {
          src: '/video/ballMan2.mov',
        }
      ],
      bw: [
        {
          src: '/video/midTerm.mov',
        },
        {
          src: '/video/finalProject1.mp4',
        }
      ],
      finals: [
        {
          src: '/video/cheeseMockUp.mp4',
        }
      ]
    }
  },
}
</script>