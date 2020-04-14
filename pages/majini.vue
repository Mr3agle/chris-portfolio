<template>
  <div>
    <v-container>
      <v-row dense class="mt-10">
        <v-col cols="12">
          <v-card color="white" light elevation="0" class="pa-10">
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar class="ma-3" size="225" tile>
                <v-img
                  src="https://lh3.googleusercontent.com/Kz0EpUTanE3sCsZcNn_b4PJmg9b5_rI1G3MVbSqCl-J2i4vNSK0L9E700z_Ouka1z5PzJakZAi4glyHrFnkNpK5hTOI81z1lEFLyi2t0OIIdiZIHtnB0YLCnUIsKB2_1EVw6_4FaAptr0pib83VlpVHjWvmyfD9nVG7u4fEXRlrKpC3Iz_qL8PA4knSTC5yMipDyC_xOaRYB2AU7smcxKvldkS0_Fh0y_YoIJF28gLwK69wlmRPNs2aBRpx-RK4jGSECl5JP82ZB6zeyP38hTIqi6PW5TN2pfMMkisE8nMw9gGfNOnwTWcwyOavfjv2SGw__yr-UpXO6IU-UJgRNW6mq38qv6aO4fSGMcPgaVONOHN9ueHEhdhGqzpw1-ytdsmYLorfZeLDzf6uPux4_C_nJN2H9XMDlX3CznH7nDmQZJ6QAbEJlhoPwyc6TxBiAFs5f6dCw4jOULhd5xSJsOJ2-ziS4B1_AWLhH5kN-sDlPEgfhNKRmMHGlPyYS6TU74la95PmyP_PdIEAgVEBylJd5uutwquPmGbq4lWOw-pA7_6pU_I8VmX6NjUV3MWQhCMLHxvkG4MXdEPHbNGE8XuITkSOWMQ6agArmDjcw21pYqJ2CYeWr_j3EH4gCVyDtACU04G0iQYcy5Xe0hFS74yfrmPCFvN9pMPKrcuDUtFUaXEPo3dsTGnw11g3Su3ww5R43qu9Y9R-0qkpgbES6T4MlzddTTnhmg03-NK0q1v073_1GiezM_U8=w1278-h719-no"
                ></v-img>
              </v-avatar>
              <div>
                <div class="section-title ml-5">
                  <img src="img/majini-title.png" alt="ApeBash" srcset="" width="150px">
                </div>
                <v-card-subtitle
                  class="pt-0 section-title-1"
                >Majini es un juego que cree como un ejercicio universitario y deriva mucha inspiración de DOOM en cuento a mecánicas y usabilidad. En corto, el juego trata acerca de matar zombies y recolectar una llave mágica que le permitirá acceder a una carpa magina y pasar el nivel. Aprendí y disfruté mucho en el desarrollo de este juego.</v-card-subtitle>
                <v-card-subtitle>El juego fue desarrollado en Unity y programado en CSharp para Gear VR. La mayoría de assets son externos y de uso libre con algunos creados por mí.</v-card-subtitle>
              </div>
            </div>
          </v-card>
        </v-col>
      </v-row>
      <v-divider class="my-6" />
      <v-row>
        <v-col>
          <v-card elevation="0">
            <v-card-title class="section-title text-center">Videos</v-card-title>
            <v-row>
              <v-col>
                <video class="px-3" src="/video/Majini trailer.mp4" width="100%" controls></video>
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
      <v-divider class="my-6" />
      <v-row>
        <v-col>
          <v-card elevation="0">
            <v-card-title class="section-title text-center">Screenshots</v-card-title>
            <v-row>
              <v-carousel class="my-5 px-7" hide-delimiters>
                <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src"></v-carousel-item>
              </v-carousel>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
      <v-divider class="my-6" />
      <v-row class="mt-7">
        <v-col>
          <v-hover>
            <template v-slot:default="{ hover }">
              <v-card class="mx-auto" max-width="300">
                <v-img
                  src="https://lh3.googleusercontent.com/8Xfxyl9gZf5lWVzj62iCFZyGQt0F6yq5WTQBGJPKRPSRLEfa0uE-fvtxvK70MwQmy3bm77OmGf5mLhzu9agcNceVIN_YkQ7MUtqXJArfqLkrqh6bzxXg4EszLlk5JZnNRZYnfN8u8Q3ZpWvQcZKHnlu1RCS4Uc1mgoIwlqpk9iluYFDsRJeHbehBAMvLmnDbwzngxmDmRRo9XdnbFS2RgfZwa1y-X-ejkBfibQjWQtBffnCGlLgDq5TnqKw2K8uarOUFYMV8uP__oijCwxqqfxomCSmNGHQGDI-lpQukt9kWEAQ2l0ILMhncJS4gBkLKz0IVtI9RPCglUOhpWXbhcEkq0aEcN3CGpXWkvEiPRsYGVybgCtnSgYcVLo-tBEyZw7Bu3Nvz5yBAjZHQ7LicZO6UpRE0zVRPGsdcBWwATidtqrnBp91Unw9ktb-XmFDwenWrrAyE0z4qJl-6aLAkXmrio1otQ4pYrCSWj46AMd1g9PfhWuxKJDhdIdicSrfIo5dwF_jjBjxCFhmWVNLrASvHobAsJRrwQPx1Isk3qXrksexW13apFZrpAveltxqOKh4daNFrQ3MtWeBc7kOSGlv64viU4YIPKomclZp7HxSoeNZoF7tHZflchZnLJI6nfqUN2KFCm3SwGkdOtyuUxbCMCmocilEuKTizDg4QnizTkqZMlK0OnioHGzg3gYQYjU8NJ_0n8r7Wx-3owT7OW8LjdNhQ7Q4a9uFRcDYV_FO_AZOWkSU_7x0=w1278-h719-no"
                >
                  <v-card-text>
                    <h2 class="section-title2 white--text">Ape Bash</h2>
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
                <v-img
                  src="https://lh3.googleusercontent.com/W6pIrXL4eYBVXfa9sQ9OFHUvyC-AfXY9XKaYcMRPm3F2kVstWaJ7QoGHI1l7pC7j0UENqEGuFcmAt_MPwhtu-5hP1g-VXhNMzlv5vcZoF331Efl6UL9cnyioil928exQUP38dQzNfhYWUGs_mvjT6WWKkp_5Qqnkx2EvzpXypdvc1cNQxGtS10S2D_CCH4r18AZEPf1C3SbbtkvJNyyy-bJvERCd93jRWGwpdCHzNcJuyHub8udhTV3i-g9dDfY5oClmTP_RVmWmeRRxy2LMskl6wqxTTs8FQ2EFUZ4CeTQJQtro5t0jhQEaDeNuzq5L8hOXPJ32iuuT4ZqY6NeI189zZ2NSj3Dto167GoDEyCtrsWdqUiysQE56FVmXwnauIFJ2xUl53G4j3m0Q8GD8880oTYiewy5PdPdo4WloIcsap2Wbl9N_3ET2mXOt5QnAIh3o_6oitjk4ddJpYtN7ApnS8eiscGy6wVbR-Vf6vcHqAnG1L0aOzhk8XgwDVLtM_-oObCbxjEdHdQioU75j87Lm-Z0hd6LH-YLbCXnp_syJEGja7ucx07aJv3CWZDVdBht9RducCgtli9jSslSVZ1PNGvwLsZg_L4Czp3l8a7ZqAWzfDZ24ju8gkxTBd_vLgawt7umyCjpWw7TAxN0KZwm-gpJtjijdgCbv1iKkqtFd5Xyxxgp92mWpcf6-80SzuLy7kqAM_NT8A1vjRYa1ZGax3ML64v8eNxZwwndxorkO7OdMpXOkDXI=w1278-h719-no"
                >
                  <v-card-text>
                    <h2 class="section-title2 white--text">The Witch</h2>
                  </v-card-text>
                </v-img>

                <v-fade-transition>
                  <v-overlay v-if="hover" absolute color="white">
                    <v-btn to="/thewitch">
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
  data () {
    return {
      items: [
        {
          src: 'https://lh3.googleusercontent.com/Kz0EpUTanE3sCsZcNn_b4PJmg9b5_rI1G3MVbSqCl-J2i4vNSK0L9E700z_Ouka1z5PzJakZAi4glyHrFnkNpK5hTOI81z1lEFLyi2t0OIIdiZIHtnB0YLCnUIsKB2_1EVw6_4FaAptr0pib83VlpVHjWvmyfD9nVG7u4fEXRlrKpC3Iz_qL8PA4knSTC5yMipDyC_xOaRYB2AU7smcxKvldkS0_Fh0y_YoIJF28gLwK69wlmRPNs2aBRpx-RK4jGSECl5JP82ZB6zeyP38hTIqi6PW5TN2pfMMkisE8nMw9gGfNOnwTWcwyOavfjv2SGw__yr-UpXO6IU-UJgRNW6mq38qv6aO4fSGMcPgaVONOHN9ueHEhdhGqzpw1-ytdsmYLorfZeLDzf6uPux4_C_nJN2H9XMDlX3CznH7nDmQZJ6QAbEJlhoPwyc6TxBiAFs5f6dCw4jOULhd5xSJsOJ2-ziS4B1_AWLhH5kN-sDlPEgfhNKRmMHGlPyYS6TU74la95PmyP_PdIEAgVEBylJd5uutwquPmGbq4lWOw-pA7_6pU_I8VmX6NjUV3MWQhCMLHxvkG4MXdEPHbNGE8XuITkSOWMQ6agArmDjcw21pYqJ2CYeWr_j3EH4gCVyDtACU04G0iQYcy5Xe0hFS74yfrmPCFvN9pMPKrcuDUtFUaXEPo3dsTGnw11g3Su3ww5R43qu9Y9R-0qkpgbES6T4MlzddTTnhmg03-NK0q1v073_1GiezM_U8=w1278-h719-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/zNkkqDFTebV61uCXsiODKjOGk-5-vPyhRpOBBDbwX3WyDNG7bK0g5IWDCHYRchS51Ity1RaBzmQSxlJ-5Uef86Sud3HFOuDk4rkHlqEEZr1sK0abbPcVegq0lMrfBhdSOvJH0VyjYJj_KGWmhI3JRDXTSUCkC8YhRSGsNqzLux46iVapDI93Vx2Nr6-Df68w-eb0yzUfPQ8eo0PtG0AFfMe2wA2I2nVZTawjsmXrfQVRoBQbJghPWx7EGLAfhl5ZBA1-CnFevTKEeilJPd2tcMjwQiTeOfjOe4GovvuWmm9z5IC9aiHhI39fGJnejiX2SQ-jdF9zwueOq4jxxkSGvjnclvL0Ng1f2RMUMbwYwsTeptXJDF46P3fKorRGIlaolS77U4_70kRugG7H31NaMvRTDpc_1zLKUYxYmuXS7D29IOndOi8SPP5BYhEAvjLoUi5wFlhFjJ5osD84LAfW38xwiBoZm9OOO7IdvoUtb33nUHKNQQ1AIFtkvPMKFP4VIe-DJwu4_LgO19gOGMoT-26wT21vNi3bDKD0bXPl7fvIeMCciTNRPQzxy2NTr3ZSupR6q91mptSjjt9PJPvAF1j1WpRRnSv3K6Pe_53DcQ0a8-TH2bB_RXLH_sKe5TCJttiymvCXUuaiDmHwNhLazg7WFFkpRnpcVchYQk2FUUVvC5J1DobUUIN_rdq2vD_DRJglYW0VIXKkQjx6anRzDrkSi_FcDfIZqOw9VVWUtYeLGhQQ44IAMJs=w652-h367-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/Y7gFXtvdaxoYLsjKu0KwSLCq29NjraNKq8znoe3Lh-_E8BaYIoO5hQx0B6mTULwKvMgtM8Zp14WpdwYV03pS8r8uARXBFaBnuf0tDgL7HivzKVLHxf72gEhDT39qnA3hF_fvMJB_XeDJ9e6pKIV_6PQ-7azDpEARUQrRr-ZcWLDdLqISSiDagfVRADhKG29qPuHcvsWK_ASdxamIZvs85gb_1GH4QFhBzuSMn2xcE5RpDKsG9MBbDCdKM8x1BEsK-jnhywEZ3LXSSO-nSMcCKeooJ39WZBf4H-pAYd9FV08PZ8ZroyKZDFHByEPXiYQywYO_29vj6Nmv2f8rGPFtEiIInISTCsvcGrjTMKdoOM0KDemWKYdmgkSMTVfGezpJaNVyk9OKRj-OwV97dGOv7NDnYcIvj-Q0LMmMEeU1PCkRpTZEiX0WORyeknqE4e27u-ABpmCFVYOnAsqVq9QaRNsSZpjufo0Nc0fk4QtdpNk_BJXfCiXrbzmZlkluVMGNPSSdbJ_zp3Htt8XYZxih6YuV4QpYZts3OuYSoLTj6ZQI1mbl0WfQkLGs6xEXzRlkCzjdAbUTWAhCvYyEzD7skedcCYLLzvosXx1fAHgB9BDXdt_jOZ2_-6bEnTvf73gYa_rInaCeKZRLRPW1LRe2trZHDEiy2E92CHN4zdTcKXZAjcOoXnmv3KbRrWxOwJOYbYbqZx934g2a1JQ7V1Y2h6UuOBb17MMrWb5pvD5H8fYvLEncCknzeo0=w653-h367-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/wjcxz7uyV2OQ_ubh3HIC3lZXX1un5s4SXRayTbrPSNCc4vRl5jDtUwEGtnEkGP-I0JO9VKpyIcNUitPqYfBuDjG-uEyjJXFNbSclE2_AHJPfUDnaSqsaslbVg8imV2YxZPnPL2c-VAIia-GJUeLABKp385XUT1qPbCZ5tzJrhGjDJQzdyPlw2_1Nqs2CdTeGkAP4_AdEXeIh5sbLa1wkUlFewwEjmUBvtQQcYt-aLdaCcctYB0kFP3w98qS8SetRKypRnbW63a8ATXtbGdEKTO316EoRni_O5dRhrQIBUD6kqulc29LPcHeKdiGHSMs0jPuDS7-ddgEYCboyWbdd7bDTKRu6zXN6i6N5i2NXxq81-EZx9zW3XfYVjbvsdbPZ-pMSlGjETjIGRpi5Zap1FYJu3btKYpdQAxAkSa6m9mcdnB-4m_fceUL42mwV2lYHJOBubPVPY08XftYz8BH9tayU2RZIjLLxypz6pJCuWn41tGesMVTOqD1G4Sa0QowJhQEtkkYBdjhwbuHr4fgcJxhOQk5-Gn1OfzZhTtkeRLmnKIplxvwOKpmtzrXuEIdE8cGq90xLbtKLMNaLaGwzf7kL8wV2Wt8j9hR8oHKr-c9E2HlTTUjCeY9FW8nmQHORr2OxigLjrWXLU8CwTupVD1L6UKq9pgXisGGYbYG26sqhd8fQ7zLgFjhov-fd4wsJQZvJISP5BsKhtLZ39AIOuhn1Qo95qR2eh8gRwtyqOfPTZmBWhpeNTJ4=w1278-h721-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/X6Bffu1mBwAphshA2NS9GCdYwEjceQ9tEy32P0jwq2qNeHVG62POBsyV3MlvAVql4KUxkl8RCfq7j-6K3KH6fYuMNoaNp93dVhze2F5HF-wfPg1WKGWue44mptaE6hxeA37wpuaxXtIS9AiULJfg4BZGYz2hZJaudwlVpj_qMxEpFdfGhCWMzYK-Dj5G2RYL5RJEGl1gcLNSqDeFH3QmNEqQr0csmpQWr0mlCNlyP0D13jPVOXm08r9fI3mwnNyyKq7En3TYELzoiriZA6ktJ5iJCyvYxSqkB80JLCVljii4tqJ4kjyLzuU5SGdDIRVXFOqmmCIhxVCsQ-UpmJviBqEAI8udFLJBIrGVHrv5t3HhyawbwR1G2azTZe8vYmPrk4LUoJFqcXTgtUJxl0u2Mzwg_xPqSbqU7ayORLaTwSNdse_W4BdQ6GzWcSfNvoCwaqQNwwCEI0moNcNXMeYC39L0CjoyR6Zr8rAl4aCB1BqnmVaJOapNxh3yI759rG5UvGUgj34R_YlrmAewWAcYs_5w5pJcxdWDPQ4n5LyCTXffAHevzXTRdxGeCiLDi1g7mv620TTuiNFkJ_SwqodeAE5_U9K0QYU0yhiPLc-fAevY_Ln8Py50p-kGkgsqq0EYpiTU4n3r7_y-UChy8wquFtZEQp80ZdpUokdyEiwfQfjv0bB8PBk_SIj1HJ0QM1EjJZXeXOY7yDknICm9JuoXQXzE6-KUiEqqa1bH1j8xW4JJMNssZLxLFdo=w652-h367-no',
        },
      ]
    }
  },
}
</script>