<template>
  <v-app>
    <navbar></navbar>
    <v-main>
      <router-view/>
    </v-main>
    <Footer></Footer>
  </v-app>
</template>

<script>
import navbar from "./components/navbar";
import Footer from "./components/footer";

export default {
  name: 'App',
  components: {
    navbar,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
