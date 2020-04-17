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
            <img src="/img/ChrisQuinnProfilePic.jpeg" />
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

      <v-btn icon href="https://www.facebook.com/christopher.quinn.5817" target="_blank">
        <v-icon>mdi-facebook</v-icon>
      </v-btn>

      <v-btn
        icon
        href="https://www.instagram.com/invites/contact/?i=166w0hx1w3v3&utm_content=fcun1p6"
        target="_blank"
      >
        <v-icon>mdi-instagram</v-icon>
      </v-btn>

      <v-btn icon href="mailto:christopherquinn10@yahoo.com" target="_blank">
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