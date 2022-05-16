<template>
  <div class="home">

    <Presentation></Presentation>

    <v-container class="mx-auto py-0" style="width: 70vw;">
      <AboutUs style="margin: 100px 0 200px 0;"></AboutUs>
      <Convention style="margin: 100px 0 200px 0;"></Convention>
      <Service style="margin: 100px 0 200px 0;"></Service>
    </v-container>
    
    <CallToReserve></CallToReserve>
    <Contact style="margin: 100px 0 200px 0;"></Contact>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import AboutUs from "@/components/about-us";
import Presentation from '@/components/present.vue'
import Service from '@/components/service.vue'
import Contact from '@/components/contact.vue'
import CallToReserve from '@/components/call-to-reserve.vue'
import Convention from '@/components/convention.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Presentation,
    Contact,
    AboutUs,
    Service,
    CallToReserve,
    Convention
  }
}
</script>
