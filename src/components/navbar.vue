<template>
  <v-app-bar
      app
      color="white"
      light
  >
    <div class="d-flex align-center">
      <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://doctormesarina.com/wp-content/uploads/2018/09/dr-alejandro-mesarina-logo-header-3-300x106.png"
          transition="scale-transition"
          width="200"
      />

      <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
      />
    </div>

    <v-spacer></v-spacer>

    <div class="hidden-sm-and-down">
      <v-btn class="text-toolbar-btn mr-4" to="/" text>Inicio</v-btn>
      <v-btn class="text-toolbar-btn mr-4" to="/profile" text>Dr. Mesarina</v-btn>
      <v-btn class="text-toolbar-btn mr-4" to="/services" text>Servicios</v-btn>
      <v-btn class="text-toolbar-btn mr-4" to="/update" text>Noticias</v-btn>
    </div>
  </v-app-bar>
</template>

<script>


export default {
  name: "navbar"
}
</script>

<style scoped>

</style>