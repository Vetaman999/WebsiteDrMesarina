<template>
  <v-app>
    <navbar></navbar>
    <v-main>
      <router-view />
    </v-main>
    <AppFooter></AppFooter>
  </v-app>
</template>

<script>
import navbar from "./components/navbar";
import AppFooter from "./components/app-footer";

export default {
  name: 'App',
  components: {
    navbar,
    AppFooter
  },

  data: () => ({
    //
  }),
};
</script>
