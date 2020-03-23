<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-card>
        <v-card-title class="headline">Bienvenidos a mi portafolio!!! 😁</v-card-title>
        <v-card-text>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Non ipsam dolorum molestias earum autem iste natus cumque quibusdam! Error quasi aliquid, molestias repudiandae facere vel expedita. Fugiat pariatur impedit necessitatibus?</p>

          <p>Este va a ser un muy buen portfolio.</p>
          <div class="text-xs-right">
            <img src="@/assets/logo/chq-l.svg" />
            <em>
              <small>&mdash; Christopher Quinn</small>
            </em>
          </div>
          <hr class="my-3" />
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn class="mb-5" color="primary" nuxt to="/animation">Proyectos</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {

}
</script>
