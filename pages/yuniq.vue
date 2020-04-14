<template>
  <div>
    <v-container>
      <v-row dense class="mt-10">
        <v-col cols="12">
          <v-card color="white" light elevation="0" class="pa-10">
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar class="ma-3" size="225" tile>
                <v-img
                  src="https://lh3.googleusercontent.com/88yEytEzHSujNx58DmWBtDhJoI7NQ1UgJJOgF26jywuViDZWyJAvKGWhZLQSo_ehYGND0p3THD3CBulIPRpRdQ233YOZy6WZkzYD7ldXrE_Jh56_r8tLpuQbrnvzBRwwXk357RkItGiyzIxhi8TgMChRPYQhNiJe_oSw2_J_sPH3uVp4e_Ks334_MAikR8d9C9Dq6B6fddkW5AfkbVt9dXIk4H5LXqys0Bwky5qRdlTagByCdlCZAgZp2I-LNh8Y_RCa7vgcFDcUrTJJbA0ealiqyOg7aufOktmv0R4qsTiRSzu9Uf0LIgBg-w_MMT4j-skOovedc3qi5PPsB9SvyuomDuJv0AEmTjFBx_XdCfODOs-VuesUqenjS3MHRy5iO9w76URxq7G3Rvx5E7Zm5H0AdbgTYa7O4BTFVJeS2MKQpot9-KeKUYxblEgb8gVhzJt_zfgpOninlO3h-5C5uBUNZDup0rTeq4Alikg_zEO8yyrqLHpls3dNFYndXm0Zx5VYBsy6wctP6HMPS1hrmJXuuW1nruuanOylEbIfIvXBDcsBqZXPxtuOAl_A1CE5JytnfsV1Zd8g7jgtVyj_xfUGy-h7wlWqTJlo_PGqYdzc57kSUN0CgBGELHNY5fnVqe83JUozlrZMTWymA14_mjdvOJOhkSNmc_uChNRPX3ECb88LOczeDsmfy5ADEcBmPZldWOvYjbH4-V50wIinNiKJxzXFbA7cQAfmybdjlCx01AfSBYHsb_o=w395-h787-no"
                ></v-img>
              </v-avatar>
              <div>
                <div class="section-title ml-5">Yuniq</div>
                <v-card-subtitle
                  class="mt-1 section-title-1"
                >Esta app simplemente fue un diseño para la app de la maraca de productos naturales Yuniq, contiene varias funcionalidades como menú de comida, carritos de compras y secciones de rewards. En el diseño prevalece el color verde para destacar la naturalidad de la maraca.</v-card-subtitle>
                <v-card-subtitle>La app está diseñada exclusivamente en Ilustrador.</v-card-subtitle>
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
              <v-col class="text-center">
                <video class="px-3" src="/video/yuniqWalkthrough.mp4" width="25%" autoplay loop></video>
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
            <v-row justify="center">
              <v-col cols="5">
                <v-carousel class="my-5 px-7" hide-delimiters>
                  <v-carousel-item
                    v-for="(item,i) in items"
                    :key="i"
                    :src="item.src"
                    max-width="250px"
                    style="margin-left: 5rem"
                  ></v-carousel-item>
                </v-carousel>
              </v-col>
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
                  src="https://lh3.googleusercontent.com/5RfeQyoY_PGXe9gk8Dtj4d4hgUXLw11oY5tSmg-249wZ3xq3ib9bV0L2nLNgZ6sE_R5rE9eVkqO5aK1MenVDkRd38ZQJQlCQSZ2BFdUoUVFk0wu9-YUezcwd52CXgeqKl3yntteQanZQqSNeJWrwNBpvBF-4MWfrw6nHjN0zlXClZC-upxenvVJkJz8FgYLYLIh4zMWMPe6HSFHHy4W3DFRUaYhZ8Snl0_MvY_2RsS1a4yasu3xOgCJvmQGgccXJkwaFpLoh6ZnIoDi_xPCdfXZRgibjRkrhUkqXYRHA-XbKrDKYCWcn5XFQ8lAY-jzKFzjQk36LeFeUhh-M6yh0TbF37L_XBAnINI0u-ASZlC0UUUkVqpqBJsrZEaKTywysA0xoKb5wuGUnkz98cpnws1J8KRaI748mTKzlEhxPKgNHXG8oyCpLj6zB0ZsrlMLQo_tT8PzjTHH_hMjlBOdWDU_l72NKQI87KpL0VKZOsVXfAgj71UP6v1rmItO3uUhN0qtMwcfwEi7r5PNCiBjKCmcl_XH7BdEsarmp9MG6tzqXu2Rg5nkWRMNw8Nb2V0Zvo8j4cUcEinzflBhCGQIRqGys48qs2IfERl1AZt4necsY1opfvFo9O8lCoPPvC5cbgVz4htpgc6sD8UhKB7nEBcEfhchSQg9Zj1tkcR69Mi6ZSzb8uqZj95IH4PTo5QGm_R2Wfv1lYJn9fR7LBzBDuiEmWMY_dot4foJsSIyS3fHfYWPuFBMvQcE=w1532-h846-no"
                  height="200"
                >
                  <v-card-text>
                    <h2 class="section-title2 white--text">Ecommerce</h2>
                  </v-card-text>
                </v-img>

                <v-fade-transition>
                  <v-overlay v-if="hover" absolute color="white">
                    <v-btn to="/ecommerce">
                      <v-icon>mdi-chevron-left</v-icon>
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
          src: 'https://lh3.googleusercontent.com/88yEytEzHSujNx58DmWBtDhJoI7NQ1UgJJOgF26jywuViDZWyJAvKGWhZLQSo_ehYGND0p3THD3CBulIPRpRdQ233YOZy6WZkzYD7ldXrE_Jh56_r8tLpuQbrnvzBRwwXk357RkItGiyzIxhi8TgMChRPYQhNiJe_oSw2_J_sPH3uVp4e_Ks334_MAikR8d9C9Dq6B6fddkW5AfkbVt9dXIk4H5LXqys0Bwky5qRdlTagByCdlCZAgZp2I-LNh8Y_RCa7vgcFDcUrTJJbA0ealiqyOg7aufOktmv0R4qsTiRSzu9Uf0LIgBg-w_MMT4j-skOovedc3qi5PPsB9SvyuomDuJv0AEmTjFBx_XdCfODOs-VuesUqenjS3MHRy5iO9w76URxq7G3Rvx5E7Zm5H0AdbgTYa7O4BTFVJeS2MKQpot9-KeKUYxblEgb8gVhzJt_zfgpOninlO3h-5C5uBUNZDup0rTeq4Alikg_zEO8yyrqLHpls3dNFYndXm0Zx5VYBsy6wctP6HMPS1hrmJXuuW1nruuanOylEbIfIvXBDcsBqZXPxtuOAl_A1CE5JytnfsV1Zd8g7jgtVyj_xfUGy-h7wlWqTJlo_PGqYdzc57kSUN0CgBGELHNY5fnVqe83JUozlrZMTWymA14_mjdvOJOhkSNmc_uChNRPX3ECb88LOczeDsmfy5ADEcBmPZldWOvYjbH4-V50wIinNiKJxzXFbA7cQAfmybdjlCx01AfSBYHsb_o=w395-h787-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/Q2LwdI0Cf0b-2yl6uxwrcQGqOgYpgKiiACvFcj84Qlr6A2bZqu-L2uUxnyB82H1gJGoRHwzCz7xrF91OCNKPDbUpC-SzAFt6-ZUEAcUcSgeKHQRH8pBbCNXqlt5lFfsZ8cl85-aRrTypV4jFSB9jX0CFFOyAZ0qDhiunkb5ncMOwhdRe37BmxvVdMYfVoNCGlHYM7ZglRfW4nFb7XFMS4FDb6V9U7Do3rIZmgIchgKi2N-DBz1C33_RSJxQDSkvviXnNnHjVnQE5M0RFWD_sZfm3jY2iDRi3CumMtVPVBj6ilg4EoR4IwtrKjZJTJq-g3XxfRpSmpzXehCwnHe6y40yT86Ggjq1UaoNWGWLxmo3tH5TdVr2XMaIpBQv4IAzBjqJG6GQGPuhuBy1JQjkqzRnB4opa2x-V40cfyKdwQssIXFDMH-AYgc6s1RrcVv59IS4wl7U5IaiUJM4FuODA42RaPLfNebZD75BZz9j2Ks4MNC5TIVZC7wHfdrkTiM3rox6lGuATLgbfXXBHZsmz0AhpFAXAN5rX_jxMHZ1FKMq6yZcxlOiv4Gd6glt9fL78BRkCtfy2palFx8ycOlgdzAwLcv5EAcTtYhGONd9vK6QNWnet9vniWXMdDscoNLWTjgNy44PiP2_9FAKrrnuBn0wlXfxHL2riGy-pVRGhUa-eqhzQGxEst3t85Z6R4ApXvsr34FC6NAypNX-RWzins5PPZArGnMAzA6t2RCQ1S6N5u-pDjcpgxoA=w389-h776-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/2Z7dy4S1dhNxhBsj6XkVwRNu86NPh3mVL2mc8Q8Ni4m0VfPu8Zft6zaxfsXjJiSsLECjP6eEmkcDcc60cPQlO040yJCW13BBBIl5n78seGrUKpGCOFbBuCAXa8rxCyi1wO0tf8UjmndWJk6zWOGOkHj8j0oWjH_fT9zmuSesfw4mvTr-ucs8s0I3CpE1fAnfarWlNMvJZ18s8EU3kmB3tPGnFe2kzxlkeLLSCNibcOBrjS5OdHILd9He1rsNrroRuSXD_vQCUbdVaAtSIalUWyUDnJNzwt8zRbY79dF8tgd3pvjNqQnQhiItacepX9lp-5UjNCYh7U70XzOLxRDCV1jNMJCfTXzSTCxzh5jt8khwcDgHG8lCOPq5403t3ax_yDQyJ-aldUAhmPlhlP8LarPsCqmjViZkDHLuB4_JP-igm5QkA6lNCIXn4iZI26vbwQueCnmWlx1UMHQWNLOp-gq5VvSv72wrTzFaP8NRqo1FzrDluNi0S_mw8G3w2-DDSfz-ZQwG3CcrFtBU-NQeCnl9Vu0nzoIRozDydz95wAshAhC8BpabIIEewb2ziHppoaz5km8U6galXuoEkpVfqdWaqxrWZtXnre2Ubpm0hotuvc7iVK84FLunIgyPh6t0ne6o7MS9WNr_82VBujOzOQBHnZ_V-Z2q9z8czZXkz5OjoAu15iaGB4Y9k6-gjXK5Hd3R1GDga32cX6R5Q_D0HIBHu3TrQ9lOz_18PGMItUs7azsxjW5x8vI=w391-h775-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/xZ7Tz1z34H8qYVPpHF-migqLutYTybua8yxOSBvWpoKjT5BTD-ENDc6wsw8rXF50cqCuHkrenCQx4vRqwkIFkhlJDhO02DNfHyoRcB1Q2-UoQ173gCtM5GbllSJ26IJGxppkcrqTIVhf_i122SE1u0N5ZqjeAmFxGRpmrEcD8ZG9Vzfz9aNM8Pb130iqdQKUIHnYMi3Yv0B1HOYXRRs5w_p3oinme-rNtGR0zxa80HczYnChR0O3VMk6PEq0RPWIhtJtbaTXIf_BLyAKKRbaJgdAg4q-93o8DW1e1vK4Ul9DWjQdu1gP7v4GH3WsrG68f7ZOgdLjdbclDB3VvJwm_SYq58ByIbxrl71M3ySTEST9q6AvTkgffe595eUwK3qKilErpt_2gpPjPah7-CzEfilmZikOtEI5NiCKojt0Mm9LeBtf13bQDOGc0gVDTgP4FPHr_CYitb1gT7_9ZIHGibPCNKpzacqUNVlaI65Ua7lWhBwuh6wcjShs-0AdNfUAeK692O6M84dF4BIMYJqfCeeGCFcKETXiecxecCvwTSGDGTVZ-GWj7YRNeuEpPRJsj3nRFF_4fLoJxQbOPbwRM5LarYz7QdWGDfkuyrOoqtlmrtzcShC9m_4jhvK0nV1t6L9r-PeTsnB5jcCJPqSAKP42xITBV5KHG0-zHusL0_Pxm2RPOcTlem9FwkrIa4EtlVWJgdfhcS-7MpB6WpIx_1OYBKMpEJVcB9ixOWoQ3aR6tylLu8pG9P4=w390-h778-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/SGURsB9GVACaciEgJUwfEc-XU0vj5pga_yx35INdQ5TYtETWJXGm5XaggjpPYCN3ULni187IazHV1fHGvKKiZhBTYfSYfp60pZV8nFAkXmsUqKhE0WegFcxbk1egIYLyFgoBN4ClcZP1smgLrqvXr51VodCPIDAbq_o0vSZLVZ8mZpcQlZd1o2FUZaNzzEzlLdvjYdhHKuz1gPSvFX2ZndBRSWm6h95uxBnNKKHCGRy9MDilHDaxXlmyS1yjdlsUMWlkr9ZSRWLwmigcGf8QXImc2RD-PgUaCSlenSrqZXiVI9ZhhrNaP1EfdhHLXPKlAH9PqwijqrMTZwe_a-E6wifJg1ToQ7oZ_pzadejuFSwuosfP96DDe_8qeT5i6jjdJNFpRABScGN4pj2HIagzwsIzSYxn9mN8dhtpfc7oeDLP9ugqbfO0q6ROArA7p6HNM4w0YuXgbqG0MnMLqOT5nB8b5AX6P7VNaInAK5MMOyfFw7k29ii9Y7GOJ-OofKGnetCRRFn-P2MnJ5ehoBnB_Hy4FJ2J0ARTayc26Eor6QJTKijIuTJoaSWjJ25a-Ygjm6kSPQOUJyHnZROGqcgSLLqvB-I7PtT5lhW20ohJg7JNuarThTPFhP8SeML4b94nji0MCHK_fNwSHLZ8O669y5HWnu0XeayDpcH8S4eDB_K-MjRKKcscLIlU2d-7nRmpFQvrL-9xwJLWJePVH4WvL1T8RNNKTzhIWdvLFoh0x3BlHp4XEM2UK8g=w387-h778-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/yFWu5DZKy5zAZjLCiNIohwVCrvc21JPeaRIOikQ1W1JO6wvanjzPFHx_2oa_FdGf-8kQ6-yBcBQ_nCPJXfL2rfzgc-uC2xiTt5ISYRNRrVrUWQJIBab8Pa1hs4lAh6U2qpqSVZtSnvOPH-kITUWihUYSUKAbq6b44Ss80eh-nB6MqNeCPAbR__BZ_Db3IY7Wnk237oPS94L8xpHSEtD5KF5oFUsv50JUe4kXDZGkgatSZ3DHmuaqYMY3vbsk-4gWnAM9RZAYhCLaKZBEXAGGG6jWLB0s2GmEsZVk4L1UHFO9XcK4sjULykKH4fMIvwvhEqUMO8A1UL55vlugvZgcyucBXPaG_iKSdPnYfGhgx1dxA8pNgG3vnJFIVxZo8SOhDtpBkM8Bxp0dPiTznZD1EHFPnht4iO7qCDU1odyh2HrPrEVfkS5cY67T7-AwWmIYL_4OufzqUjfD1gvWQivplwmTrEd3Diyj5_e7fyKAubwhqjQhI_o0JEH7cbjvHnVRFLKspENWUGDYQAFavtaCi0bAH60PN0AtlGWyewu3viuliTh49HO2uiAdoZxsCuYAW-i-NNPx3cF3cgbLHYmDvdRHnwV16lfrteBFaw5clPDYhzQ14sTswXyayjGGBgkZ6Y4TAzfFS7aCq0Pkxw_CWAlzmd8_WqMhHzOhfu2gEHCbeTi_iSMoFP8KqMFqT53NWLM6mUxwoHWOVntc-OUGCeCmuMy10RPrdfhI9Sv08dkpTZWBXakG8nM=w383-h777-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/VlxM00-24CnxkbZkUld3tBHXIoecbAeTWT53nHe1BhXmiqEsGuB1o8CEmnDkeubE1rKMvnDO1fVClHsT0rn2Srm4AVyqDLWkZDXWei7Djw0ZFo5sTesINO74v-SQJfIzUrG5UrBb0LVnqf3cKQqhXGgNsdVVj17VmT661seqZQVXt8NyrcAfnrYX3ZuA_q1Nc3l69sycbwomY_JVg7EnhE_z7P_XcyXGGNdH1lJhNJIhYbrbU2zuY2NUap_xCnyvzppQ3i32YUYZQUmGbBMAoJPS9u3oFNkkBoOXE7Oop5o2bTPcM7gYt_UmQVSin-iEO8FRrT8lNYgTPnmrI0aIFl-S3wObgYoTzLpEfDLUhse_GFN5tkKOYOe3Tp4Vp6NuedTjF0d3VCI6vi68FRMyE-Mmalg9gPi4DuwoL-eD_P4toYib5YYnQ2hZTrCZVdkauNU7su2WiIWvMGOv5fN7xoOAUhrBT_aF1OjUFcbtmp3KgbRhRpQlzPVNF5_w4VX7_oWnNLV-8z20MYWSWAC_jtNf_ske17za56uWxgWf2mXh1UOxBSEpNFeHvwumg_iMZLe7cBLYlLzK7Rxg25XDuFV2QTrydWevx57q79XaaFjDg3UM5CjOS8ZtD5xPXGGy90fen3MK4w6Ziq7PbalEHwoWPnu409S-Z37nJr5VxHdQwSONG-0YQ_anXlEsuxznw1VHl87Hw3qMZWpySPaVRx1ShdvGGFW38Cuv1EDmmUvziIHM5yd2f-U=w393-h777-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/3ru_1EOHCAd-Non37ybbsWvl7DSx5NwaxTQ9Pb1u9LaZeFffOlPso87LMjxMmIKWrlhUu_uFfQ-87ll6Y8xwyg28-SjYrg5RR1pV7bPweWH2sypPVRtzbeorKU1xcZEx0AQ293nckTcH6ywD1rhFyM7V75wJNIcs1FVaRTfgJPnhVagu4YU-QAbUFvy_UjiDIboIbpyIoPJvmiW-FLzRWQit36B1sJRSnAsi14IdzU-0DUHEONtAb4V-Rm2P6JZXce990vOPgLnU2xR_w69g8QTU33URQAwjLHbm1rlT9r0uyXBWIsWpbrMl7qF9ko8FnYdS3oPvNg7zk_0tvZkEpHqb3PjgutTvw777ojdciFidxTh3IhKgA27JNJYtgWMe5sWEHY0vdrzxt8NejqKolg4r48Q_NtpEvvcnznvuCqKbPmsWoLCS2kEy1wEwCmtQRNV4s71qSGbLDS8AUagal_9xgDsHxkJCllZva39VOHbIlw_dpwXSoKwcZVKw-NQqXI_PGkZyO2_iZ7FI53kj28QFRGGQXDvOR44OCHa0zOR2WX_8q8v7h25QDlLkmdeC3Aqf21Z_7iP7lh1Bsu4SBQZLO0nGWMgdLxrfJqRH0SrVUoonAn49kTKqXUc7Ze65nmebfguuawTeZypCUu6-C4JHd9_r5XvMGEo9Zl7MbOlPY1ZdrQnut0yS4Bg8M8qfylW2n4Obfp-4_A7NKpq3_lZiunQeUhNWHl4ekfiDCcDMPhgri0mNhvo=w384-h778-no',
        }
      ]
    }
  },
}
</script>