<template>

  <div>


    <v-container class="mx-auto py-0" style="width: 70vw;">
      <AboutUs style="margin: 100px 0 200px 0;"></AboutUs>
    </v-container>

    <CallToReserve 
      title="Llámanos para reservar tu consulta"
      subTitle="Si tienes y quieres una consulta... Llámanos con toda confianza. Nosotros lo vamos a ayudar"
      btnText="Llámanos"
    />

    <v-container class="mx-auto py-0" style="width: 70vw;">
      <Service style="margin: 100px 0 100px 0;"></Service>
    </v-container>

    <Contact style="margin: 100px 0 100px 0;"/>


  </div>
</template>

<script>
import AboutUs from "@/components/about-us";
import Service from '@/components/service.vue'
import Contact from '@/components/contact.vue'
import CallToReserve from '@/components/call-to-reserve.vue'

export default {
  name: 'Home',
  components: {
    Contact,
    AboutUs,
    Service,
    CallToReserve,
  }
}
</script>
