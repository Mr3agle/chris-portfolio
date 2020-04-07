<template>
  <div>
    <v-parallax
      dark
      src="https://images.pexels.com/photos/2653362/pexels-photo-2653362.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
      fluid
    >
      <v-row align="center" justify="center">
        <v-col class="text-center" cols="12">
          <h1 class="banner-title">Web&ndash;Dev</h1>
        </v-col>
      </v-row>
    </v-parallax>
    <v-container>
      <v-row dense>
        <v-col v-for="(item, i) in items" :key="i" cols="6">
          <v-hover>
            <template v-slot:default="{ hover }">
              <v-card class="mx-auto my-5" :color="item.color" dark elevation="15" max-width="500">
                <v-img
                  :src="item.src"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="400px"
                >
                  <v-card-title class="section-title-2" v-text="item.title"></v-card-title>

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
  </div>
</template>

<script>
export default {
  data: () => ({
    overlay: false,
    items: [
      {
        color: '#1F7087',
        src: 'https://lh3.googleusercontent.com/5RfeQyoY_PGXe9gk8Dtj4d4hgUXLw11oY5tSmg-249wZ3xq3ib9bV0L2nLNgZ6sE_R5rE9eVkqO5aK1MenVDkRd38ZQJQlCQSZ2BFdUoUVFk0wu9-YUezcwd52CXgeqKl3yntteQanZQqSNeJWrwNBpvBF-4MWfrw6nHjN0zlXClZC-upxenvVJkJz8FgYLYLIh4zMWMPe6HSFHHy4W3DFRUaYhZ8Snl0_MvY_2RsS1a4yasu3xOgCJvmQGgccXJkwaFpLoh6ZnIoDi_xPCdfXZRgibjRkrhUkqXYRHA-XbKrDKYCWcn5XFQ8lAY-jzKFzjQk36LeFeUhh-M6yh0TbF37L_XBAnINI0u-ASZlC0UUUkVqpqBJsrZEaKTywysA0xoKb5wuGUnkz98cpnws1J8KRaI748mTKzlEhxPKgNHXG8oyCpLj6zB0ZsrlMLQo_tT8PzjTHH_hMjlBOdWDU_l72NKQI87KpL0VKZOsVXfAgj71UP6v1rmItO3uUhN0qtMwcfwEi7r5PNCiBjKCmcl_XH7BdEsarmp9MG6tzqXu2Rg5nkWRMNw8Nb2V0Zvo8j4cUcEinzflBhCGQIRqGys48qs2IfERl1AZt4necsY1opfvFo9O8lCoPPvC5cbgVz4htpgc6sD8UhKB7nEBcEfhchSQg9Zj1tkcR69Mi6ZSzb8uqZj95IH4PTo5QGm_R2Wfv1lYJn9fR7LBzBDuiEmWMY_dot4foJsSIyS3fHfYWPuFBMvQcE=w1532-h846-no',
        title: 'Ecommerce',
        description: 'La página fue desarrollada en PHP, HTML y javascript, con una base de datos MySQL.',
        to: '/ecommerce'
      },
      {
        color: '#952175',
        src: 'https://lh3.googleusercontent.com/88yEytEzHSujNx58DmWBtDhJoI7NQ1UgJJOgF26jywuViDZWyJAvKGWhZLQSo_ehYGND0p3THD3CBulIPRpRdQ233YOZy6WZkzYD7ldXrE_Jh56_r8tLpuQbrnvzBRwwXk357RkItGiyzIxhi8TgMChRPYQhNiJe_oSw2_J_sPH3uVp4e_Ks334_MAikR8d9C9Dq6B6fddkW5AfkbVt9dXIk4H5LXqys0Bwky5qRdlTagByCdlCZAgZp2I-LNh8Y_RCa7vgcFDcUrTJJbA0ealiqyOg7aufOktmv0R4qsTiRSzu9Uf0LIgBg-w_MMT4j-skOovedc3qi5PPsB9SvyuomDuJv0AEmTjFBx_XdCfODOs-VuesUqenjS3MHRy5iO9w76URxq7G3Rvx5E7Zm5H0AdbgTYa7O4BTFVJeS2MKQpot9-KeKUYxblEgb8gVhzJt_zfgpOninlO3h-5C5uBUNZDup0rTeq4Alikg_zEO8yyrqLHpls3dNFYndXm0Zx5VYBsy6wctP6HMPS1hrmJXuuW1nruuanOylEbIfIvXBDcsBqZXPxtuOAl_A1CE5JytnfsV1Zd8g7jgtVyj_xfUGy-h7wlWqTJlo_PGqYdzc57kSUN0CgBGELHNY5fnVqe83JUozlrZMTWymA14_mjdvOJOhkSNmc_uChNRPX3ECb88LOczeDsmfy5ADEcBmPZldWOvYjbH4-V50wIinNiKJxzXFbA7cQAfmybdjlCx01AfSBYHsb_o=w395-h787-no',
        title: 'Yuniq',
        description: 'La app está diseñada exclusivamente en Ilustrador. ',
        to: '/yuniq'
      }
    ],
  }),
}
</script>