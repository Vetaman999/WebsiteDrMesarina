<template>
  <v-app>
    <navbar></navbar>
    <v-content class="mx-auto py-0" style="width: 70vw;">
      <v-main>
        <router-view/>
      </v-main>
      <Footer></Footer>
    </v-content>
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
