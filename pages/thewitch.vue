<template>
  <div>
    <v-container>
      <v-row dense>
        <v-col cols="12">
          <v-card color="white" light elevation="5">
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar class="ma-3" size="225" tile>
                <v-img
                  src="https://lh3.googleusercontent.com/W6pIrXL4eYBVXfa9sQ9OFHUvyC-AfXY9XKaYcMRPm3F2kVstWaJ7QoGHI1l7pC7j0UENqEGuFcmAt_MPwhtu-5hP1g-VXhNMzlv5vcZoF331Efl6UL9cnyioil928exQUP38dQzNfhYWUGs_mvjT6WWKkp_5Qqnkx2EvzpXypdvc1cNQxGtS10S2D_CCH4r18AZEPf1C3SbbtkvJNyyy-bJvERCd93jRWGwpdCHzNcJuyHub8udhTV3i-g9dDfY5oClmTP_RVmWmeRRxy2LMskl6wqxTTs8FQ2EFUZ4CeTQJQtro5t0jhQEaDeNuzq5L8hOXPJ32iuuT4ZqY6NeI189zZ2NSj3Dto167GoDEyCtrsWdqUiysQE56FVmXwnauIFJ2xUl53G4j3m0Q8GD8880oTYiewy5PdPdo4WloIcsap2Wbl9N_3ET2mXOt5QnAIh3o_6oitjk4ddJpYtN7ApnS8eiscGy6wVbR-Vf6vcHqAnG1L0aOzhk8XgwDVLtM_-oObCbxjEdHdQioU75j87Lm-Z0hd6LH-YLbCXnp_syJEGja7ucx07aJv3CWZDVdBht9RducCgtli9jSslSVZ1PNGvwLsZg_L4Czp3l8a7ZqAWzfDZ24ju8gkxTBd_vLgawt7umyCjpWw7TAxN0KZwm-gpJtjijdgCbv1iKkqtFd5Xyxxgp92mWpcf6-80SzuLy7kqAM_NT8A1vjRYa1ZGax3ML64v8eNxZwwndxorkO7OdMpXOkDXI=w1278-h719-no"
                ></v-img>
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
                <v-img
                  src="https://lh3.googleusercontent.com/8Xfxyl9gZf5lWVzj62iCFZyGQt0F6yq5WTQBGJPKRPSRLEfa0uE-fvtxvK70MwQmy3bm77OmGf5mLhzu9agcNceVIN_YkQ7MUtqXJArfqLkrqh6bzxXg4EszLlk5JZnNRZYnfN8u8Q3ZpWvQcZKHnlu1RCS4Uc1mgoIwlqpk9iluYFDsRJeHbehBAMvLmnDbwzngxmDmRRo9XdnbFS2RgfZwa1y-X-ejkBfibQjWQtBffnCGlLgDq5TnqKw2K8uarOUFYMV8uP__oijCwxqqfxomCSmNGHQGDI-lpQukt9kWEAQ2l0ILMhncJS4gBkLKz0IVtI9RPCglUOhpWXbhcEkq0aEcN3CGpXWkvEiPRsYGVybgCtnSgYcVLo-tBEyZw7Bu3Nvz5yBAjZHQ7LicZO6UpRE0zVRPGsdcBWwATidtqrnBp91Unw9ktb-XmFDwenWrrAyE0z4qJl-6aLAkXmrio1otQ4pYrCSWj46AMd1g9PfhWuxKJDhdIdicSrfIo5dwF_jjBjxCFhmWVNLrASvHobAsJRrwQPx1Isk3qXrksexW13apFZrpAveltxqOKh4daNFrQ3MtWeBc7kOSGlv64viU4YIPKomclZp7HxSoeNZoF7tHZflchZnLJI6nfqUN2KFCm3SwGkdOtyuUxbCMCmocilEuKTizDg4QnizTkqZMlK0OnioHGzg3gYQYjU8NJ_0n8r7Wx-3owT7OW8LjdNhQ7Q4a9uFRcDYV_FO_AZOWkSU_7x0=w1278-h719-no"
                >
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
          src: 'https://lh3.googleusercontent.com/-Td71C8lxQaU5-xNfBvdEguOwhuZmqFVaEsSi8yZl8Aoz-s54JqSk5lXXTJgF1g0tJcNFtU8afPisLQHJE0-4dgVdXdrnCqnKAPw0Wr3C0AWQzwkcc9Pgn10SAUCd2AjaKuPyH02peZET4IK80BNvFgVHl48YWW2cIhnEafVNTGDDoqKpHsTNFdaRGVkjoZJRPlzmf6wXfPUNt49en0V_oFrGBB_ii-ZnZaSdydBrdHxIcLNOhS4VA-4c1gu8ZCpVZ-nDQvCCE49rgByIDxOUDIurUrFrLFzzAvTt7Llr-S8-1-b7KUPyx696IXkIg-evC_0F1CZ-WCPJzdUZEgI2Sbt_Mf4lhArLUFQAXS6A8rPB1mNF30Llk2RgTDZS-dLtCG4HDcYpvKGOqxl9eIaGoVibOphl0qWe0bKsgqzbl-ADAwaeepu1kqQOabWUnM7rl4V09tCd6CQtHq6ehaRxLMqt3K5vkfWyLLULFQ8SW-c-4EJuBqCWp4p6oAMOAdtiQvXDzMqCVBtoKK_FEyMFT4i8fuUfJDbGI1j6Av-zbPS0y4MtVTo42blsKKGbQNNE7O2HoS1LAoKFMcbxXtcBal7lKjllUVAhrobpq-pnrhFnuJUpg7aLcrdWmlC8BPs9b_y9k1qvdKFSWWZeqDFvBGgIf6To53Cz2BszCA_7M5LiLT8i6yCuFgwfopjxVlMlJCQZOgkFdaCxGZZChDArdoNeXRPVaojHNZKvV1tm_09UTQhMBDekEc=w1278-h719-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/W6pIrXL4eYBVXfa9sQ9OFHUvyC-AfXY9XKaYcMRPm3F2kVstWaJ7QoGHI1l7pC7j0UENqEGuFcmAt_MPwhtu-5hP1g-VXhNMzlv5vcZoF331Efl6UL9cnyioil928exQUP38dQzNfhYWUGs_mvjT6WWKkp_5Qqnkx2EvzpXypdvc1cNQxGtS10S2D_CCH4r18AZEPf1C3SbbtkvJNyyy-bJvERCd93jRWGwpdCHzNcJuyHub8udhTV3i-g9dDfY5oClmTP_RVmWmeRRxy2LMskl6wqxTTs8FQ2EFUZ4CeTQJQtro5t0jhQEaDeNuzq5L8hOXPJ32iuuT4ZqY6NeI189zZ2NSj3Dto167GoDEyCtrsWdqUiysQE56FVmXwnauIFJ2xUl53G4j3m0Q8GD8880oTYiewy5PdPdo4WloIcsap2Wbl9N_3ET2mXOt5QnAIh3o_6oitjk4ddJpYtN7ApnS8eiscGy6wVbR-Vf6vcHqAnG1L0aOzhk8XgwDVLtM_-oObCbxjEdHdQioU75j87Lm-Z0hd6LH-YLbCXnp_syJEGja7ucx07aJv3CWZDVdBht9RducCgtli9jSslSVZ1PNGvwLsZg_L4Czp3l8a7ZqAWzfDZ24ju8gkxTBd_vLgawt7umyCjpWw7TAxN0KZwm-gpJtjijdgCbv1iKkqtFd5Xyxxgp92mWpcf6-80SzuLy7kqAM_NT8A1vjRYa1ZGax3ML64v8eNxZwwndxorkO7OdMpXOkDXI=w1278-h719-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/FUCU7LlZbqhcvmMUKogXT7KdrYYL4VkE6zgIFFU88HJDqX91cMtJV-YyfqBcSqkjPXctYFk7VrQZrqI7PQRCA1snnqB44wMY8VNZkxEXCxNQn9yJpC9Uf3YwICbeNnKBUiXSps5iUBbenf67ntV_IufxUPF6DQk1rodgR2lrm8ZTL1ok79PKdhy-6oAHaKn6NWNCJEB4Cv6UgyOS-lmWhgn5Mx7nluIuKFftJLJMLYrHRAILuQCdxJOO2BMr3_olurBN3EpB41r8yILZNDpheFyveRQy3zC42FAWRjiyVxj1hBmO4mtuBj8-rT1ZwNCpZG9xnadIclzP7xlmLqrEbHayUnlMDDbDBI_2ZUapN5ZMbJWJVProg4FFvnHXJBwzrOggoNFA7Q87F4Kt_36KqMcs2pdi7vTXVoYEjzn3tbnIluDLC5lFgKR0XNDXEMnj358J3aTwedi5Xt43MZCUjGnj1pDbUdGQiRNq-8RfD-as2rzyPlNlHvXNW1oVsBCBTZ93O0xNlHjIgp8p7zC5Iq_quRP0EyTSmXWEotOzp3OxTGDmgb8e7fdC_-qaMZWoCUlc1AV59EveDgkw-ouStNYFjBniZXjfGXS9x5NDxKT6j5mN3f6qMkHL1zIHT2f7D8kyRNm7uMTQr8k2OcyC6kj1DvC5rmlRXxZdckTHL9DW-rUhybOFQsP6z-L4-7gnphkgDhx74a7ovPH8KS91xCYZus3QRgmN9tubywLzM_7e77svGmKnTj4=w1278-h719-no',
        }
      ]
    }
  },
}
</script>