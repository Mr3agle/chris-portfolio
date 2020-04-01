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
        src: 'https://lh3.googleusercontent.com/_nlDTBPh4XaqfUwrJXckJsrNF8b_GOfdROMuYshq_7Vmj5Kol3NRoB-INHmG2ziYdIQskvUW9uI_fPnZj5A121FYmRxBdFn82FVuVQb3NNbwDXa_q8pOzMFO_26ZludKScU6me9PXIpAEcg0ttvnBn1MEzqqBQDxbfHz5FNajaUmM5ivwD8g5vm8G37Gb8m2IabJwiFPLilXYW4s30GvE7AAK7uRacoPsZB7XNnd2dZlCuz5HZg5vEwUSSGe5XtGd5dFChpm0TNJnr9u-w3gfbBtYyFxNrNNJYq3f7Pqw_IF9--IUshgSeQTyvDxXNkHdt4PhkHUNgdYYqGfN-nlr40zKYs18GsR-2hMpu1TcNNsyWNb4Vz0FXY9VjlQZWlloFcMY-r3Rh1WNoI-R-1QeRk_72vK8GQ8Rrv4NzOr2alYmYhXeaS6kNOxq_8sg0CKGuyI4ipVCfsoH4EpY1JeORvGt0oh1XRSiXbECe4vCrSP08l1MF-NCbW_ZzefIN9FRq3_NceHTFP0iSpxWxjE2bCFwKTJ0PB2hO82cxSRlzsAc8pGXyKI43rb_IckksIVbHYf4IATprZw4n1NXfrIXmXl9Sa_6JO5ilSK_cwU7GFBTSHWBwJV7e6zCWwYhPlDiwkkaFAZPmNw2IFnBSdcmTPfkp4rrL6465WldssIvxZXgyiqaNfWyivNFluVSiPbOnDpe0YZOLYGrldyh5oYeThHlRKWFzFfFYmSFJZBtQeo4cxPHELywJQ=w1278-h719-no',
        title: 'ApeBash',
        description: 'El juego fue desarrollado en Unity y programado en CSharp. La mayoría de assets son externos y de uso libre con algunos creados por mí. ',
        to: '/apebash'
      },
      {
        color: '#952175',
        src: 'https://lh3.googleusercontent.com/Kz0EpUTanE3sCsZcNn_b4PJmg9b5_rI1G3MVbSqCl-J2i4vNSK0L9E700z_Ouka1z5PzJakZAi4glyHrFnkNpK5hTOI81z1lEFLyi2t0OIIdiZIHtnB0YLCnUIsKB2_1EVw6_4FaAptr0pib83VlpVHjWvmyfD9nVG7u4fEXRlrKpC3Iz_qL8PA4knSTC5yMipDyC_xOaRYB2AU7smcxKvldkS0_Fh0y_YoIJF28gLwK69wlmRPNs2aBRpx-RK4jGSECl5JP82ZB6zeyP38hTIqi6PW5TN2pfMMkisE8nMw9gGfNOnwTWcwyOavfjv2SGw__yr-UpXO6IU-UJgRNW6mq38qv6aO4fSGMcPgaVONOHN9ueHEhdhGqzpw1-ytdsmYLorfZeLDzf6uPux4_C_nJN2H9XMDlX3CznH7nDmQZJ6QAbEJlhoPwyc6TxBiAFs5f6dCw4jOULhd5xSJsOJ2-ziS4B1_AWLhH5kN-sDlPEgfhNKRmMHGlPyYS6TU74la95PmyP_PdIEAgVEBylJd5uutwquPmGbq4lWOw-pA7_6pU_I8VmX6NjUV3MWQhCMLHxvkG4MXdEPHbNGE8XuITkSOWMQ6agArmDjcw21pYqJ2CYeWr_j3EH4gCVyDtACU04G0iQYcy5Xe0hFS74yfrmPCFvN9pMPKrcuDUtFUaXEPo3dsTGnw11g3Su3ww5R43qu9Y9R-0qkpgbES6T4MlzddTTnhmg03-NK0q1v073_1GiezM_U8=w1357-h763-no',
        title: 'Majini',
        description: 'El juego fue desarrollado en Unity y programado en CSharp para Gear VR. La mayoría de assets son externos y de uso libre con algunos creados por mí.',
        to: '/apebash'
      },
      {
        color: '#952175',
        src: 'https://lh3.googleusercontent.com/qdB_xUmc886w_kXvNt_g3UkJSCW_18OyOdjU95UAAPsn-A-YtY1vUpkRFPW7Kgas-unjgX5mioWtvQ7lCVC355CM4oiz-9ESK1Qp0VZbqz_eCyyRH8iNIvQaWaWrfIjnUe7DFAwRoZRyW3cvMs0rz0eEGhacsky4jWeuuseFjQt8jMxBEOmPWkltDgi65XKk8mjHWM1KYOUvk1RZzRrKOXwY7mw8v2H1-CiWWkZ6M33VEGSsFLUAuMdWajKJbGEJSojpGbQgvdoeV05ZrFKLtYiQ8F17_IG3q9rA3bheNS90-palOi4Tf5VExWGQ-nHDfOx0Mb97uKXfRS55iOxobNes3CBQ5wCElr4E2lgfay9pfWpGySYryOvAWWIWdi37bNers5DyFXWKX-bGAhJtuQ05em5BQLidLBJ4TLe-MvAshGM012Wig4_NSRNgzXAwwBc7jEqAZiWIjiV3cAn_QEZ5f2U3VkPcNr-ul8pDrKU6gBKhyoz1VDNGdaz_yhcd6-_QPxpg1WVnGIvzssGW6_P2GlLov3TzEUSsAK3Iivu9zQzi-JPqRX_KrNYlCEnk6Fjne8b8N_uNSlGSE1qkGE8WswtLpLkdbcRKM8t3DdkJ5lDox8caA0DdUd9JI9tmGVTYslGNMER38OxwpMfwnrHJOM6bi-Bdu_qppMiLGvhVIdO3XUZEKGb2PSOHARSym5Ze2pAVqnTwwNjHe4JEEFnJLK8DCC_YoMxQfne3EliB9E0dQkksyDI=w653-h367-no',
        title: 'The Witch',
        description: 'El juego fue desarrollado en Unity y programado en CSharp para Gear VR. La mayoría de assets son externos y de uso libre con algunos creados por mí.',
        to: '/apebash'
      }
    ],
  }),
}
</script>