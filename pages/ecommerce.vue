<template>
  <div>
    <v-container>
      <v-row dense class="mt-10">
        <v-col cols="12">
          <v-card color="white" light elevation="0" class="pa-10">
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar class="ma-3" size="225" tile>
                <v-img
                  src="https://lh3.googleusercontent.com/5RfeQyoY_PGXe9gk8Dtj4d4hgUXLw11oY5tSmg-249wZ3xq3ib9bV0L2nLNgZ6sE_R5rE9eVkqO5aK1MenVDkRd38ZQJQlCQSZ2BFdUoUVFk0wu9-YUezcwd52CXgeqKl3yntteQanZQqSNeJWrwNBpvBF-4MWfrw6nHjN0zlXClZC-upxenvVJkJz8FgYLYLIh4zMWMPe6HSFHHy4W3DFRUaYhZ8Snl0_MvY_2RsS1a4yasu3xOgCJvmQGgccXJkwaFpLoh6ZnIoDi_xPCdfXZRgibjRkrhUkqXYRHA-XbKrDKYCWcn5XFQ8lAY-jzKFzjQk36LeFeUhh-M6yh0TbF37L_XBAnINI0u-ASZlC0UUUkVqpqBJsrZEaKTywysA0xoKb5wuGUnkz98cpnws1J8KRaI748mTKzlEhxPKgNHXG8oyCpLj6zB0ZsrlMLQo_tT8PzjTHH_hMjlBOdWDU_l72NKQI87KpL0VKZOsVXfAgj71UP6v1rmItO3uUhN0qtMwcfwEi7r5PNCiBjKCmcl_XH7BdEsarmp9MG6tzqXu2Rg5nkWRMNw8Nb2V0Zvo8j4cUcEinzflBhCGQIRqGys48qs2IfERl1AZt4necsY1opfvFo9O8lCoPPvC5cbgVz4htpgc6sD8UhKB7nEBcEfhchSQg9Zj1tkcR69Mi6ZSzb8uqZj95IH4PTo5QGm_R2Wfv1lYJn9fR7LBzBDuiEmWMY_dot4foJsSIyS3fHfYWPuFBMvQcE=w1532-h846-no"
                ></v-img>
              </v-avatar>
              <div>
                <div class="section-title ml-5">Ecommerce</div>
                <v-card-subtitle
                  class="mt-1 section-title-1"
                >Esta fue una página que cree en conjunto con Adrian Maguiña para promover y vender su marca de ropa. En el cual existen varias categorías de ropa, además tiene un carrito de compras funcional en el cual se puede comprar y pagar por medio de Stripe. Además, el proyecto contiene una página de aministrador, el cual puede añadir nuevas categorías de ropa, stockear la ropa existente y confirmar ordenes de envió.</v-card-subtitle>
                <v-card-subtitle>La página fue desarrollada en PHP, HTML y javascript, con una base de datos MySQL.</v-card-subtitle>
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
                <video class="px-3" src="/video/site1.mp4" width="100%" controls></video>
              </v-col>
              <v-col>
                <video class="px-3" src="/video/site2.mp4" width="100%" controls></video>
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
                  src="https://lh3.googleusercontent.com/88yEytEzHSujNx58DmWBtDhJoI7NQ1UgJJOgF26jywuViDZWyJAvKGWhZLQSo_ehYGND0p3THD3CBulIPRpRdQ233YOZy6WZkzYD7ldXrE_Jh56_r8tLpuQbrnvzBRwwXk357RkItGiyzIxhi8TgMChRPYQhNiJe_oSw2_J_sPH3uVp4e_Ks334_MAikR8d9C9Dq6B6fddkW5AfkbVt9dXIk4H5LXqys0Bwky5qRdlTagByCdlCZAgZp2I-LNh8Y_RCa7vgcFDcUrTJJbA0ealiqyOg7aufOktmv0R4qsTiRSzu9Uf0LIgBg-w_MMT4j-skOovedc3qi5PPsB9SvyuomDuJv0AEmTjFBx_XdCfODOs-VuesUqenjS3MHRy5iO9w76URxq7G3Rvx5E7Zm5H0AdbgTYa7O4BTFVJeS2MKQpot9-KeKUYxblEgb8gVhzJt_zfgpOninlO3h-5C5uBUNZDup0rTeq4Alikg_zEO8yyrqLHpls3dNFYndXm0Zx5VYBsy6wctP6HMPS1hrmJXuuW1nruuanOylEbIfIvXBDcsBqZXPxtuOAl_A1CE5JytnfsV1Zd8g7jgtVyj_xfUGy-h7wlWqTJlo_PGqYdzc57kSUN0CgBGELHNY5fnVqe83JUozlrZMTWymA14_mjdvOJOhkSNmc_uChNRPX3ECb88LOczeDsmfy5ADEcBmPZldWOvYjbH4-V50wIinNiKJxzXFbA7cQAfmybdjlCx01AfSBYHsb_o=w395-h787-no"
                  height="200"
                >
                  <v-card-text>
                    <h2 class="section-title2 black--text">Yuniq</h2>
                  </v-card-text>
                </v-img>

                <v-fade-transition>
                  <v-overlay v-if="hover" absolute color="white">
                    <v-btn to="/yuniq">
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
          src: 'https://lh3.googleusercontent.com/5RfeQyoY_PGXe9gk8Dtj4d4hgUXLw11oY5tSmg-249wZ3xq3ib9bV0L2nLNgZ6sE_R5rE9eVkqO5aK1MenVDkRd38ZQJQlCQSZ2BFdUoUVFk0wu9-YUezcwd52CXgeqKl3yntteQanZQqSNeJWrwNBpvBF-4MWfrw6nHjN0zlXClZC-upxenvVJkJz8FgYLYLIh4zMWMPe6HSFHHy4W3DFRUaYhZ8Snl0_MvY_2RsS1a4yasu3xOgCJvmQGgccXJkwaFpLoh6ZnIoDi_xPCdfXZRgibjRkrhUkqXYRHA-XbKrDKYCWcn5XFQ8lAY-jzKFzjQk36LeFeUhh-M6yh0TbF37L_XBAnINI0u-ASZlC0UUUkVqpqBJsrZEaKTywysA0xoKb5wuGUnkz98cpnws1J8KRaI748mTKzlEhxPKgNHXG8oyCpLj6zB0ZsrlMLQo_tT8PzjTHH_hMjlBOdWDU_l72NKQI87KpL0VKZOsVXfAgj71UP6v1rmItO3uUhN0qtMwcfwEi7r5PNCiBjKCmcl_XH7BdEsarmp9MG6tzqXu2Rg5nkWRMNw8Nb2V0Zvo8j4cUcEinzflBhCGQIRqGys48qs2IfERl1AZt4necsY1opfvFo9O8lCoPPvC5cbgVz4htpgc6sD8UhKB7nEBcEfhchSQg9Zj1tkcR69Mi6ZSzb8uqZj95IH4PTo5QGm_R2Wfv1lYJn9fR7LBzBDuiEmWMY_dot4foJsSIyS3fHfYWPuFBMvQcE=w1532-h846-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/Ku_yfj72hifLAdyqYpS08CPSuzUMLMhLB85aRnE3teGMw_DIXnt--h0FPYADjR3XQIC7Db-eq3Gfm4tRCjOUF6IEeJdG0bydDThe7y3PpEbWPOgRxeiy0pYZTDHANml3aaYY2AFwMITTteOdVo1WNbqkq3xAjUkClOuoRC4gu0RAIj22WLQB_LObUoveiZflZNr41Yg2CPyIb_65CfpwHMP7fCj2bg8o3y0fserLmOx05pPKf0FJEowWpGiMJirj5mshcQ2fkdJIRjW91HY0hWL-o9BNQYLyqLjNcMpNJzc5ZgWcZLGPibhWescTJP9BcQadI8hw1qH0NDt-pNLMPDOiD1lH2d2dHdnjJcVuv3DA3OF97EoTGXDVthOwr3LqPKbdjyiWYLbSQ--yZplfi64ZaFp2xhieBXMEU1pDg6gix89NIsklroCQ0sRqjSQa4ilecT_ATXNwiEBSge4iKS_iAQTqOKSdI0StNGviCZ2mA0yoi0S2o5xhu5ASAj3SVeL_sLQheOSA6jzGavsJekm0LHUQIBm_QuYv6zjhgrDsgvst8aHPIXmUWnObro3Vq_dqKXNmjmL_VCN-NyOBHqhU0fGTnjdhetPaJE3afKvwxGxjbvyphiQY9ZRyCeeugZhf2l0ZUsOWsITph4JavQ9IdGELhGkn1yGEALH1SFGac0e51UM0gLllT_H3m2M94ACXctZmqwXN-U6vOtwwAOeKpeN7jjQswZWMeDSzqjs2V197vpRUKgU=w718-h396-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/A03ngzzNxksyD8IQmz5ddyBpqeyye12jcxEqB235gm1chJthaKdr5Gcy7c2Td6PsB0mnZwRQhVXIGdCtfcuVVonzRLUjQIVN7VZR1zEhQ-pb_SI1_YRbXBYjv757iwLJpjW4vXoBMGjbHuW_GJM0wh0JLX2jSeR0XylrL_piy84J4PkMwvwhBj68_awGhrCji51popmsZiFeHVIG0uLRFP9W2UEu2FuNcM15DkMkZGacqGD59Zkoqilj31aKINm-iUaPSnkx6AL5s6nzqU0QTpyPkHnq-EPSQ4ST4DnapWv2PzUfMn-cemqGDiJzTGI8Z9QBIbHogooWRVDBS6JjeAVdRQE6uhgEmpvf2I67Qo8weg45JSvuO02v9FvKCN4i78xwwCCozTbrYI4T1M0Og1JmfPeelaCj7mRxtaMFhaqU-yf0OGwerfhCMwAkR-9jCcWC-hLt8PcP_6fypdLmCRfF-9ZPsMIjsuHfrILtYJ6hU3sOLVrdr0sNL5X23FMAJ8uxn9TRUD114IRxPjDpuyZ2n_dAk3JbYzn8Pnvff80sMWD_bICARXvy7wGM7tRTZk_Jws3uwg-SsJZy51n1_9pxLYFo-cvz_pMUjH3QDBeH7aNWTbm6OKkeUlT9aBvQ6q2tQltY1b7-A-v_gYnUvwRba5-fbyyZwFcWBg4Tt_2DmEby0sJQg7uuYweSqXUc69GCJX1eSZVeSIVGN3YZR_TyRNkucKqYlmM91SUeXdp7PS8vHVqk0lc=w1532-h846-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/tDCmVzUfXN-GUjCmd8l08tDoDc1sKSHCWGS9Lxau7IyT65pTwhn54CQc2kSu__Zo97PjWpBeh4OzqJRUdnTxPcI0kM5x1kwSyx7ZGNFI89ygP-DjhfV10TOrf1zIPL02xaSqZSa0MFVhTs6dV2b81Y5UpoOxnCGq0vX05NHMu4NrP6an9uHkStGpKcDloPbTGaNf_ruWEdP0tA8wVGQR4TAXeGCnS0rwHhVY44Sb434uEg5TCWHjOQ_K-J3Y1DAE5iyJ8vE9xsy9UL4mK1H4W6zt9EpFJuLDa8ID_-0JRf85sQPK5nw--2xTaUEikZ9nZMOtS_tgS1eapMRoFg5EX5xnB92diQluO2s6jXwEwVbJmpZB38YZPtYbi4JoOGYw-rp1ZJYiNwDzuBlNk5yQUnyG_EZ4OFe3rEGypoUs3a4-9Ek-S3YYs3xOIzWzR41FriIX64SG96Ot6WJafqvUjHQhgWbULpVNJgXxgsUfTToD72iPHRty1mNFLhbuCOcYjvw0gVP2jxA7BiYyAH-2W7DFqBYsm6137NNlL5HA9UArHyaBY3B5_YCPdX6WB7EO0d04uOtY-wgDR-fUDHewH3VnvRjY0kczJWxIXXwoISR5fPbHbDqyTNGx7F7lzvjFCLmdhFbNov8OkkDJ-et2attse8IuBzA1Wo_VIOEBNmg91hf3YjigB5UesWVcjABX5I66iwjVskbTd8up0M-F5RKLZujkqik8Erzl4jvXrAiw-NpJLRCChy8=w1532-h846-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/V_vH8KVuu_ZyKK8Y3ZCCc03cwSpJxtV8q20jf8MY9OHVp5-ITAYJ5A1rUtBUW7n9ngRutaaO1fxmrgZRIfTupIKx1cfg9GolfE39LIn5TIkCU9wgpUGB-S6WAYI2_0ElVzvv6x_RXY1VHxKypa-ywKn183mMv4ld4Ur_qY14ugB5mIQz-J5DyswE4hPwIAR_5n_PF5zcc8YOzX22_CWadiziEgRfrdYaMch_6RV9K7QFJYO9ER7ZAesritAVExg5McjMcdnBWDlHBj2alb5wQtIP7oFopUWW1fRENHosfV4PkPE_w3jbIN67N1pAwcCtBs1SFXZlJxiGmW_qUZD4yT6Md6ejil-t0GEz_95jKwziZB50_99Jk4ZgJBdhQprCY4Hqf5eJGEMjRec1mY7jzbqEHomf17cY5Xc8tEfo-HxdH1YQ6aM5BGDlzLFpz34xpifaEAcCwl83GfhhMQm52zBC2PT5vhwKNDhemF6bPfuc1fcr2XbMZk13rSm5IFMdMRTVlIUq0NndBPFr7CrMCyjt9WfaIlO9vZJbp58XYYhWvuObDTR00BsoXqdbGUUYqd49FN0lEuWgd8OGijNq4sLa2gujSHy_oRivJJy7Y1SRHEGIUclStctF85QaypaFEz9uQzcOcfT-tQc9ZkjriiyLL5mX3SMqyMGJsxzwZpQWINEFBnG8_laqICoDLKlDUi1ZANnooalWSeFTLim_PDmbBrRn7Ee_PQqdlmXTtpXQfxA96l4R10g=w1532-h846-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/g9ydlWESRJggyRQc4jfODxxTKmYc5xqo10zNY8Ghbk0ACDJuv0H3wzvoXUWWOyjxH6s8xr--eEDodWEldf6TZkHS8KRddrStK8G5C9pJMafQNR12awKY4gbl-rIYZAX2DuUEPH9PFdXCriML0BIwtfm8S_2C4XdaPxt9rS9Q5FgmVa0pRHwVu3KsEBb9-szsefnbNaGxdvSw9wt8qxN0m46rn0ctQ-JZhsD6e_CIZaJu_zMoiFZzdVYnzHi9ckKU9WtXXbSmo-WITcA21iCvQWBrIj3f30ceo5CScw9CxVDgtrUA-qNC2JGRJcq_rkAwdKM8vZUK31gEwr0Crc1cuX5IrSsqYFGSlQIwJaFa0Ji9EIqfgpLcSgdApnEa_bHaSemjgue8-iD9B6vNn7aT99vSrLP_BrZLrpcNYfUG-dhGitZR6pAlUB2cFAiR-G505QNtzjuFTqHvq4lop82IA0-WevYJMnqnrTQShBZd_yzIwtmlgdG6GFom6srzOF7nmBuTaWlm-oFmVcZrRuzds0H3RIPamcFgmck5HUgriMHHHRhuQ5cpHt3yPf3gKjtbt6xRzTZ_0ZiL23wlIRd68Tdg9dWgrQqzy9FSSWb3MhgjlfYuc9qm1__Pi5-ILtqslwQZf3EsP_PhN5iAOPQl3bo8DmjFi3FF5hp40aG5UuVei3qHeXbkspEhTwT7LH7ouHqlCBxFuI9YtpkzwkdPR_EXgqTHnRqMKe3m5epGi8e0iOu7V-qXNBY=w1532-h846-no',
        }
      ]
    }
  },
}
</script>