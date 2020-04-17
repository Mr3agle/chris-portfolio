<template>
  <!-- <v-container> -->
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-card class="mx-auto my-10" max-width="700px" elevation="0">
        <v-card-text>
          <div class="text-center">
            <img src="@/assets/logo/chq-d.svg" width="400px" />
          </div>
          <div class="text-center">
            <img src="/img/ChrisQuinnProfilePic.jpeg" width="300px" style="border-radius: 50%" />
          </div>

          <p class="text-justify mt-5">
            Soy un Diseñador Interactivo ecuatoriano/estadounidense apasionado que disfruta de las aventuras y los pequeños momentos de la vida. Me encanta el football americano, los videojuegos, la cocina y mis hermosos perros.
            Estudie Animación y Medios Interactivos en la Universidad San Francisco de Quito y me gradué con un título en Diseño Gráfico: Medios Interactivos.
            Acepto cualquier desafío aunque inicialmente tal vez no sepa como abarcarlo siempre lo venzo.
          </p>

          <hr class="my-5" />

          <v-row>
            <v-col>
              <div class="section-title-home text-center">Contacto</div>
              <v-row justify="center" class="mt-5">
                <v-btn class text x-large href="tel:+593 98 568 6956">
                  <v-icon large color="black lighten-5" class="mx-3">mdi-phone</v-icon>
                </v-btn>

                <v-btn class text x-large href="mailto: christopherquinn10@yahoo.com">
                  <v-icon large color="black lighten-5" class="mx-3">mdi-email</v-icon>
                </v-btn>
              </v-row>
            </v-col>
            <v-col>
              <div class="section-title-home text-center">Redes Sociales</div>
              <v-row justify="center" class="mt-5">
                <v-btn
                  class
                  text
                  x-large
                  color="blue"
                  href="https://www.facebook.com/christopher.quinn.5817"
                  target="_blank"
                >
                  <v-icon large color="blue" class="mx-3">mdi-facebook</v-icon>
                </v-btn>
                <v-btn
                  class
                  text
                  x-large
                  color="pink"
                  href="https://www.instagram.com/invites/contact/?i=166w0hx1w3v3&utm_content=fcun1p6"
                  target="_blank"
                >
                  <v-icon large color="pink lighten-3" class="mx-3">mdi-instagram</v-icon>
                </v-btn>
                <v-btn class text x-large color="teal" href="mailto:christopherquinn10@yahoo.com">
                  <v-icon large color="teal" class="mx-3">mdi-email</v-icon>
                </v-btn>
              </v-row>
            </v-col>
          </v-row>
          <div class="my-3"></div>
          <div class="section-title text-center">Logos de Clientes</div>

          <v-row justify="center mt-10">
            <img src="img/logoPI.jpg" alt="logopi" width="250px" class="mx-4" />
            <img src="img/logoPixel.jpg" alt="logopixel" width="35px" class="mx-4" />
          </v-row>
        </v-card-text>
      </v-card>
    </v-flex>
  </v-layout>
  <!-- </v-container> -->
</template>

<script>
export default {

}
</script>

<style lang="scss">
.link-contact {
  font-size: 1.5rem;
  color: blue;
  text-decoration: none;
  i {
    font-size: 2rem;
    color: blue;
  }
}

body {
  background: url('https://images.pexels.com/photos/2670898/pexels-photo-2670898.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940');
}
</style>