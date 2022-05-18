<template>
  <div>
    <Presentation></presentation>
    <CardProfile style="margin: 50px 0 50px 0;"></CardProfile>
    <our-mission></our-mission>
    <CallToReserve 
      title="¡RESERVA TU CITA HOY!"
      subTitle="¿Quieres reservar una cita con nosotros?... Llámanos con toda confianza. Estamos aquí para ti."
      btnText="LLÁMANOS"
    />
  </div>
</template>
<script> 
import Presentation from '@/components/present.vue'
import CardProfile from '@/components/card-profile.vue'
import OurMission from '@/components/our-mission.vue'
import CallToReserve from '@/components/call-to-reserve.vue'

export default {
  name: 'Profile',
  components: {
    Presentation,
    CardProfile,
    OurMission,
    CallToReserve
  }
}
</script>
