<template>
  <v-app dark>
    <v-navigation-drawer v-model="drawer" :mini-variant="miniVariant" :clipped="clipped" fixed app>
      <v-list>
        <v-row justify="space-around">
          <v-avatar class="mt-5" size="62">
            <img
              src="https://lh3.googleusercontent.com/ryDCW2KLJk10pQtH3aRXIBB8aff8OaacPusUn0UxUdrOGvEF1C2blFGd11r0f3wi5Zefk0Ftx1Z2Wcm2nqu_f6loDsosrTMk0n307JmfC-bqcWFNc3H5wAS0W844VqFbO6L8aiS4pqPooy4XujACXvcsPoPBWnx6bTsi4XInKKf0zECuzvX-jlCx9ITSI_BCpIcpb1A3p5vzcCNt9KlJzMY8t-JX2vkKALBJLYhRYLcKIvzjVd-3Br0C15Pss1Sr51EkNdHEB5dCSzqHVqV_NMo7h6fajvDa2gOBF48Qelxz_q3pjkUOVm0T5gDqnEMjTOZ6xrI_VrRpvaki5skmzEPVb9CBLbXMSQq7wJojOhshFwBArg34b_ytbmzRMy38HIYSeVGdb746vYimiT6-l_uU4lHeDbZ76MTDVxCGms26dvw5Zd-LJ_tdGOf4_Jeai72Kg2HKZ_sbXGcn-TiURZhTB4D0h7r93T-s1y6VgTbinftMHD3ovSiBxG7NFaH8fM4i8bgdjqhDVRg3EqA2PZh7uF1y0a2vs9Y36fq-rxLwgRKWntF3jboguv8yMWBLTQwI-rofmMJR7dTldWYNBB0PW-CpNKDA4L1h5QwXMHAwxHDPwTNpxFxzFw_lB2V_PkRwRt0ZV9LgfrDV_4ZAZdf9h6aZ9eo56s3wtC9F8iispfF2Dc7U9G-JA0o5xI8nZQutECEbrnhjDCLpRrkScism19cNld20tS4trLknTtHPB8F4clR7VRk=w1002-h1000-no"
              alt="Chris Quinn"
            />
          </v-avatar>
        </v-row>
        <v-row justify="space-around">
          <v-list-item-content class="text-center">
            <v-list-item-title class="title">Christopher Quinn</v-list-item-title>
            <v-list-item-subtitle>Diseñador Gráfico Interactivo</v-list-item-subtitle>
          </v-list-item-content>
        </v-row>
        <v-list-item v-for="(item, i) in items" :key="i" :to="item.to" router exact>
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <!-- <v-btn icon @click.stop="miniVariant = !miniVariant">
        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
      </v-btn>-->
      <!-- <v-btn icon @click.stop="clipped = !clipped">
        <v-icon>mdi-application</v-icon>
      </v-btn>-->
      <!-- <v-btn icon @click.stop="fixed = !fixed">
        <v-icon>mdi-minus</v-icon>
      </v-btn>-->
      <!-- <v-toolbar-title v-text="title" /> -->
      <!-- <v-spacer /> -->
      <v-toolbar-items>
        <nuxt-link to="/" :prefetch="false" class="my-auto">
          <img src="@assets/logo/chq-l.svg" style="height: 40px;" />
        </nuxt-link>
      </v-toolbar-items>
      <!-- <v-btn icon @click.stop="rightDrawer = !rightDrawer">
        <v-icon>mdi-menu</v-icon>
      </v-btn>-->
    </v-app-bar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer :fixed="fixed" app>
      <v-spacer></v-spacer>
      <span>Christopher Quinn &copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
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
          title: 'Web-dev',
          to: '/webdev'
        }
      ],
      miniVariant: false
    }
  }
}
</script>
