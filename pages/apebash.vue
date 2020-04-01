<template>
  <div>
    <v-container>
      <v-row dense>
        <v-col cols="12">
          <v-card color="white" light elevation="5">
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar class="ma-3" size="225" tile>
                <v-img
                  src="https://lh3.googleusercontent.com/_nlDTBPh4XaqfUwrJXckJsrNF8b_GOfdROMuYshq_7Vmj5Kol3NRoB-INHmG2ziYdIQskvUW9uI_fPnZj5A121FYmRxBdFn82FVuVQb3NNbwDXa_q8pOzMFO_26ZludKScU6me9PXIpAEcg0ttvnBn1MEzqqBQDxbfHz5FNajaUmM5ivwD8g5vm8G37Gb8m2IabJwiFPLilXYW4s30GvE7AAK7uRacoPsZB7XNnd2dZlCuz5HZg5vEwUSSGe5XtGd5dFChpm0TNJnr9u-w3gfbBtYyFxNrNNJYq3f7Pqw_IF9--IUshgSeQTyvDxXNkHdt4PhkHUNgdYYqGfN-nlr40zKYs18GsR-2hMpu1TcNNsyWNb4Vz0FXY9VjlQZWlloFcMY-r3Rh1WNoI-R-1QeRk_72vK8GQ8Rrv4NzOr2alYmYhXeaS6kNOxq_8sg0CKGuyI4ipVCfsoH4EpY1JeORvGt0oh1XRSiXbECe4vCrSP08l1MF-NCbW_ZzefIN9FRq3_NceHTFP0iSpxWxjE2bCFwKTJ0PB2hO82cxSRlzsAc8pGXyKI43rb_IckksIVbHYf4IATprZw4n1NXfrIXmXl9Sa_6JO5ilSK_cwU7GFBTSHWBwJV7e6zCWwYhPlDiwkkaFAZPmNw2IFnBSdcmTPfkp4rrL6465WldssIvxZXgyiqaNfWyivNFluVSiPbOnDpe0YZOLYGrldyh5oYeThHlRKWFzFfFYmSFJZBtQeo4cxPHELywJQ=w1278-h719-no"
                ></v-img>
              </v-avatar>
              <div>
                <v-card-title class="display-2">ApeBash</v-card-title>

                <v-card-subtitle
                  class="mt-1 subtitle-1"
                >ApeBash es un juego inspirado en Fruit Ninja, en el que el jugador deberá sobrevivir el mayor tiempo a un ataque fructifero de hombre monos. El jugador tiene una espada para poder rebanar todo tipo de fruta que es lanzada en su dirección.</v-card-subtitle>
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
                <video class="px-3" src="/video/Ape Bash trailer.mp4" width="100%" controls></video>
              </v-col>
              <v-col>
                <video class="px-3" src="/video/ApeBashGameplay.mp4" width="100%" controls></video>
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
                <v-img
                  src="https://lh3.googleusercontent.com/W6pIrXL4eYBVXfa9sQ9OFHUvyC-AfXY9XKaYcMRPm3F2kVstWaJ7QoGHI1l7pC7j0UENqEGuFcmAt_MPwhtu-5hP1g-VXhNMzlv5vcZoF331Efl6UL9cnyioil928exQUP38dQzNfhYWUGs_mvjT6WWKkp_5Qqnkx2EvzpXypdvc1cNQxGtS10S2D_CCH4r18AZEPf1C3SbbtkvJNyyy-bJvERCd93jRWGwpdCHzNcJuyHub8udhTV3i-g9dDfY5oClmTP_RVmWmeRRxy2LMskl6wqxTTs8FQ2EFUZ4CeTQJQtro5t0jhQEaDeNuzq5L8hOXPJ32iuuT4ZqY6NeI189zZ2NSj3Dto167GoDEyCtrsWdqUiysQE56FVmXwnauIFJ2xUl53G4j3m0Q8GD8880oTYiewy5PdPdo4WloIcsap2Wbl9N_3ET2mXOt5QnAIh3o_6oitjk4ddJpYtN7ApnS8eiscGy6wVbR-Vf6vcHqAnG1L0aOzhk8XgwDVLtM_-oObCbxjEdHdQioU75j87Lm-Z0hd6LH-YLbCXnp_syJEGja7ucx07aJv3CWZDVdBht9RducCgtli9jSslSVZ1PNGvwLsZg_L4Czp3l8a7ZqAWzfDZ24ju8gkxTBd_vLgawt7umyCjpWw7TAxN0KZwm-gpJtjijdgCbv1iKkqtFd5Xyxxgp92mWpcf6-80SzuLy7kqAM_NT8A1vjRYa1ZGax3ML64v8eNxZwwndxorkO7OdMpXOkDXI=w1278-h719-no"
                >
                  <v-card-text>
                    <h2 class="title white--text">The Witch</h2>
                  </v-card-text>
                </v-img>

                <v-fade-transition>
                  <v-overlay v-if="hover" absolute color="white">
                    <v-btn to="/thewitch">
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
                <v-img
                  src="https://lh3.googleusercontent.com/Kz0EpUTanE3sCsZcNn_b4PJmg9b5_rI1G3MVbSqCl-J2i4vNSK0L9E700z_Ouka1z5PzJakZAi4glyHrFnkNpK5hTOI81z1lEFLyi2t0OIIdiZIHtnB0YLCnUIsKB2_1EVw6_4FaAptr0pib83VlpVHjWvmyfD9nVG7u4fEXRlrKpC3Iz_qL8PA4knSTC5yMipDyC_xOaRYB2AU7smcxKvldkS0_Fh0y_YoIJF28gLwK69wlmRPNs2aBRpx-RK4jGSECl5JP82ZB6zeyP38hTIqi6PW5TN2pfMMkisE8nMw9gGfNOnwTWcwyOavfjv2SGw__yr-UpXO6IU-UJgRNW6mq38qv6aO4fSGMcPgaVONOHN9ueHEhdhGqzpw1-ytdsmYLorfZeLDzf6uPux4_C_nJN2H9XMDlX3CznH7nDmQZJ6QAbEJlhoPwyc6TxBiAFs5f6dCw4jOULhd5xSJsOJ2-ziS4B1_AWLhH5kN-sDlPEgfhNKRmMHGlPyYS6TU74la95PmyP_PdIEAgVEBylJd5uutwquPmGbq4lWOw-pA7_6pU_I8VmX6NjUV3MWQhCMLHxvkG4MXdEPHbNGE8XuITkSOWMQ6agArmDjcw21pYqJ2CYeWr_j3EH4gCVyDtACU04G0iQYcy5Xe0hFS74yfrmPCFvN9pMPKrcuDUtFUaXEPo3dsTGnw11g3Su3ww5R43qu9Y9R-0qkpgbES6T4MlzddTTnhmg03-NK0q1v073_1GiezM_U8=w1278-h719-no"
                >
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
          src: 'https://lh3.googleusercontent.com/8Xfxyl9gZf5lWVzj62iCFZyGQt0F6yq5WTQBGJPKRPSRLEfa0uE-fvtxvK70MwQmy3bm77OmGf5mLhzu9agcNceVIN_YkQ7MUtqXJArfqLkrqh6bzxXg4EszLlk5JZnNRZYnfN8u8Q3ZpWvQcZKHnlu1RCS4Uc1mgoIwlqpk9iluYFDsRJeHbehBAMvLmnDbwzngxmDmRRo9XdnbFS2RgfZwa1y-X-ejkBfibQjWQtBffnCGlLgDq5TnqKw2K8uarOUFYMV8uP__oijCwxqqfxomCSmNGHQGDI-lpQukt9kWEAQ2l0ILMhncJS4gBkLKz0IVtI9RPCglUOhpWXbhcEkq0aEcN3CGpXWkvEiPRsYGVybgCtnSgYcVLo-tBEyZw7Bu3Nvz5yBAjZHQ7LicZO6UpRE0zVRPGsdcBWwATidtqrnBp91Unw9ktb-XmFDwenWrrAyE0z4qJl-6aLAkXmrio1otQ4pYrCSWj46AMd1g9PfhWuxKJDhdIdicSrfIo5dwF_jjBjxCFhmWVNLrASvHobAsJRrwQPx1Isk3qXrksexW13apFZrpAveltxqOKh4daNFrQ3MtWeBc7kOSGlv64viU4YIPKomclZp7HxSoeNZoF7tHZflchZnLJI6nfqUN2KFCm3SwGkdOtyuUxbCMCmocilEuKTizDg4QnizTkqZMlK0OnioHGzg3gYQYjU8NJ_0n8r7Wx-3owT7OW8LjdNhQ7Q4a9uFRcDYV_FO_AZOWkSU_7x0=w1278-h719-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/Ds4opJRrD-xEoFu1QCA4bPBUuWTe6XuEmmBBEMPIGX7Fn1fHpD0yaK53KUeyo4lEP6JFXOuQMP-am8qnXTZkF8HdYlv9ym1l1-XYxcwJ0yQVWKXoQvs4_frEsvK570NBaPjwqga6hFdL0JPEH9CVu6HeGcdN286gk974htA3D0fBBKAA9IrdYsYtwc196TnfTqUVRebmNAszLXwu-xw37mMn10FbcnIy5ktOyS0w8Spxah5TQ5QMLqVaiy3XVSKgsSYZf1kurULUiwoePJ2nMsNXrIpXUBRT1E_JFw-fereyYPHFcPGK1HYSdG2SsecECi3_tR0PojN_FTqWV5JsDo1plqnYj5GZhtKX-U8_q_REdDhGJQFqeoArOzGITjx70BKyq4o3dDNE00PDRXtPVRx43pVqlseMeWcpoPOy1RM6OFMfZ1VJjPdpijAPG34TMhqs9eP1TFOU5-GR4xhjz8sWF-9n-3dTkQQ09J9y8xKdet8jLW5Cwv9lYT7zn0oj7gQM8F1D7JusXdiYXcWCC_fCNFGuqCWORZXKk2iGLiD1UEGHCl2Dxfn_VR2aRbTUQBD5uocuEEn4IYi8y8bZnXlk6smF0rUULyQWpI_5LRuhFC5iNPRUELqUe3mwZPJCWawN2f_sZ3b_ST5k4EBEmMoSKCmMgo9OnShC4duaknkvuHG78WC-hEO_wcrxhmOEMkCWYlzT-uwTUBWc5AwFQNpDUDfs1XIoZyPSQdNA3ka7w_umJ7tOD_s=w455-h256-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/_nlDTBPh4XaqfUwrJXckJsrNF8b_GOfdROMuYshq_7Vmj5Kol3NRoB-INHmG2ziYdIQskvUW9uI_fPnZj5A121FYmRxBdFn82FVuVQb3NNbwDXa_q8pOzMFO_26ZludKScU6me9PXIpAEcg0ttvnBn1MEzqqBQDxbfHz5FNajaUmM5ivwD8g5vm8G37Gb8m2IabJwiFPLilXYW4s30GvE7AAK7uRacoPsZB7XNnd2dZlCuz5HZg5vEwUSSGe5XtGd5dFChpm0TNJnr9u-w3gfbBtYyFxNrNNJYq3f7Pqw_IF9--IUshgSeQTyvDxXNkHdt4PhkHUNgdYYqGfN-nlr40zKYs18GsR-2hMpu1TcNNsyWNb4Vz0FXY9VjlQZWlloFcMY-r3Rh1WNoI-R-1QeRk_72vK8GQ8Rrv4NzOr2alYmYhXeaS6kNOxq_8sg0CKGuyI4ipVCfsoH4EpY1JeORvGt0oh1XRSiXbECe4vCrSP08l1MF-NCbW_ZzefIN9FRq3_NceHTFP0iSpxWxjE2bCFwKTJ0PB2hO82cxSRlzsAc8pGXyKI43rb_IckksIVbHYf4IATprZw4n1NXfrIXmXl9Sa_6JO5ilSK_cwU7GFBTSHWBwJV7e6zCWwYhPlDiwkkaFAZPmNw2IFnBSdcmTPfkp4rrL6465WldssIvxZXgyiqaNfWyivNFluVSiPbOnDpe0YZOLYGrldyh5oYeThHlRKWFzFfFYmSFJZBtQeo4cxPHELywJQ=w1278-h719-no',
        }
      ]
    }
  },
}
</script>