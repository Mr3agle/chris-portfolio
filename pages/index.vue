<template>
  <!-- <v-container> -->
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-card class="mx-auto my-10" max-width="700px" elevation="0">
        <v-card-text>
          <div class="text-xs-right text-lg-center">
            <img src="@/assets/logo/chq-d.svg" width="400px" />
          </div>
          <div class="text-xs-right text-lg-center">
            <img
              src="https://lh3.googleusercontent.com/ryDCW2KLJk10pQtH3aRXIBB8aff8OaacPusUn0UxUdrOGvEF1C2blFGd11r0f3wi5Zefk0Ftx1Z2Wcm2nqu_f6loDsosrTMk0n307JmfC-bqcWFNc3H5wAS0W844VqFbO6L8aiS4pqPooy4XujACXvcsPoPBWnx6bTsi4XInKKf0zECuzvX-jlCx9ITSI_BCpIcpb1A3p5vzcCNt9KlJzMY8t-JX2vkKALBJLYhRYLcKIvzjVd-3Br0C15Pss1Sr51EkNdHEB5dCSzqHVqV_NMo7h6fajvDa2gOBF48Qelxz_q3pjkUOVm0T5gDqnEMjTOZ6xrI_VrRpvaki5skmzEPVb9CBLbXMSQq7wJojOhshFwBArg34b_ytbmzRMy38HIYSeVGdb746vYimiT6-l_uU4lHeDbZ76MTDVxCGms26dvw5Zd-LJ_tdGOf4_Jeai72Kg2HKZ_sbXGcn-TiURZhTB4D0h7r93T-s1y6VgTbinftMHD3ovSiBxG7NFaH8fM4i8bgdjqhDVRg3EqA2PZh7uF1y0a2vs9Y36fq-rxLwgRKWntF3jboguv8yMWBLTQwI-rofmMJR7dTldWYNBB0PW-CpNKDA4L1h5QwXMHAwxHDPwTNpxFxzFw_lB2V_PkRwRt0ZV9LgfrDV_4ZAZdf9h6aZ9eo56s3wtC9F8iispfF2Dc7U9G-JA0o5xI8nZQutECEbrnhjDCLpRrkScism19cNld20tS4trLknTtHPB8F4clR7VRk=w1002-h1000-no"
              width="300px"
              style="border-radius: 50%"
            />
          </div>

          <p class="text-justify mt-5">
            Soy un Diseñador Interactivo ecuatoriano/estadounidense apasionado que disfruta de las aventuras y los pequeños momentos de la vida. Me encanta el football americano, los videojuegos, la cocina y mis hermosos perros.
            Estudie Animación y Medios Interactivos en la Universidad San Francisco de Quito y me gradué con un título en Diseño Gráfico: Medios Interactivos.
            Acepto cualquier desafío aunque inicialmente tal vez no sepa como abarcarlo siempre lo venzo.
          </p>

          <hr class="my-5" />

          <div class="section-title text-center">Contacto</div>
          <div class="my-3 text-center">
            <v-btn class text x-large color="blue" href="tel:+593 98 568 6956">
              <v-icon>mdi-phone</v-icon>&nbsp; 098 568 6956
            </v-btn>
          </div>
          <div class="my-3 text-center">
            <v-btn class text x-large color="blue" href="mailto: christopherquinn@yahoo.com">
              <v-icon>mdi-email</v-icon>&nbsp; christopherquinn@yahoo.com
            </v-btn>
          </div>

          <div class="section-title text-center">Redes Sociales</div>
          <div class="my-3">
            <v-row justify="center">
              <v-btn class text x-large color="blue" href="#">
                <v-icon large color="blue" class="mx-3">mdi-facebook</v-icon>
              </v-btn>
              <v-btn class text x-large color="pink" href="#">
                <v-icon large color="pink lighten-3" class="mx-3">mdi-instagram</v-icon>
              </v-btn>
              <v-btn class text x-large color="teal" href="#">
                <v-icon large color="teal" class="mx-3">mdi-email</v-icon>
              </v-btn>
            </v-row>
          </div>
          <div class="section-title text-center">Logos de Marcas</div>

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