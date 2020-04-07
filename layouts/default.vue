<template>
  <v-app light>
    <v-navigation-drawer
      dark
      v-model="drawer"
      :mini-variant="miniVariant"
      :expand-on-hover="expandOnHover"
      :clipped="clipped"
      fixed
      app
      :src="bg"
    >
      <v-list shaped>
        <v-list-item two-line :class="miniVariant && 'px-0'">
          <v-list-item-avatar class="ml-2">
            <img
              src="https://lh3.googleusercontent.com/ryDCW2KLJk10pQtH3aRXIBB8aff8OaacPusUn0UxUdrOGvEF1C2blFGd11r0f3wi5Zefk0Ftx1Z2Wcm2nqu_f6loDsosrTMk0n307JmfC-bqcWFNc3H5wAS0W844VqFbO6L8aiS4pqPooy4XujACXvcsPoPBWnx6bTsi4XInKKf0zECuzvX-jlCx9ITSI_BCpIcpb1A3p5vzcCNt9KlJzMY8t-JX2vkKALBJLYhRYLcKIvzjVd-3Br0C15Pss1Sr51EkNdHEB5dCSzqHVqV_NMo7h6fajvDa2gOBF48Qelxz_q3pjkUOVm0T5gDqnEMjTOZ6xrI_VrRpvaki5skmzEPVb9CBLbXMSQq7wJojOhshFwBArg34b_ytbmzRMy38HIYSeVGdb746vYimiT6-l_uU4lHeDbZ76MTDVxCGms26dvw5Zd-LJ_tdGOf4_Jeai72Kg2HKZ_sbXGcn-TiURZhTB4D0h7r93T-s1y6VgTbinftMHD3ovSiBxG7NFaH8fM4i8bgdjqhDVRg3EqA2PZh7uF1y0a2vs9Y36fq-rxLwgRKWntF3jboguv8yMWBLTQwI-rofmMJR7dTldWYNBB0PW-CpNKDA4L1h5QwXMHAwxHDPwTNpxFxzFw_lB2V_PkRwRt0ZV9LgfrDV_4ZAZdf9h6aZ9eo56s3wtC9F8iispfF2Dc7U9G-JA0o5xI8nZQutECEbrnhjDCLpRrkScism19cNld20tS4trLknTtHPB8F4clR7VRk=w1002-h1000-no"
            />
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>Christopher Quinn</v-list-item-title>
            <v-list-item-subtitle>Diseñador gráfico Interactivo</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-divider></v-divider>
        <v-list-item
          color="white"
          dark
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar dark :src="bg" :clipped-left="clipped" fixed app elevation="0">
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />

      <v-toolbar-items>
        <nuxt-link to="/" :prefetch="false" class="my-auto">
          <img src="@/assets/logo/chq-l.svg" style="height: 40px;" />
        </nuxt-link>
      </v-toolbar-items>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-facebook</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-instagram</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-email</v-icon>
      </v-btn>
    </v-app-bar>
    <v-content>
      <v-container fluid pa-0>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer dark>
      <v-spacer></v-spacer>
      <span>Christopher Quinn &copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: true,
      drawer: true,
      fixed: true,
      items: [
        {
          icon: 'mdi-transition',
          title: 'Animación',
          to: '/animation'
        },
        {
          icon: 'mdi-space-invaders',
          title: 'Juegos',
          to: '/games'
        },
        {
          icon: 'mdi-file-code',
          title: 'Web-Dev',
          to: '/webdev'
        }
      ],

      miniVariant: true,
      background: true,
      expandOnHover: true
    }
  },
  computed: {
    bg () {
      return this.background ? 'https://images.pexels.com/photos/355465/pexels-photo-355465.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940' : undefined
    },
  },
}
</script>

<style lang="scss">
* {
  font-family: 'Montserrat', sans-serif;
}
</style>