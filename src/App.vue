<template>
  <v-app>
    <navbar></navbar>
        <Presentation />
    <v-main>
      <router-view />
    </v-main>
    <AppFooter></AppFooter>
    <wsp></wsp>
  </v-app>
</template>

<script>
import navbar from "./components/navbar";
import AppFooter from "./components/app-footer";
import Wsp from "./components/btn-wsp.vue";
import Presentation from '@/components/present.vue'
export default {
  name: 'App',
  components: {
    navbar,
    Wsp,
    AppFooter,
    Presentation
  },

  data: () => ({
    //
  }),
};
</script>
