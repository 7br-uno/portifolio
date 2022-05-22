<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          :src="require('./assets/logo.png')"
          transition="scale-transition"
          width="40"
        />
        <span>My Portifolio</span>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        icon
        color="white"
        class="mx-1"
        href="mailto:dev@7br.uno"
      >
        <v-icon>mdi-email-outline</v-icon>
      </v-btn>

      <v-btn
        href="https://7br.uno/"
        target="_blank"
        text
      >
        <span class="mr-2 text-lowercase">https://7br.uno/</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
