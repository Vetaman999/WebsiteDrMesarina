<template>
  <div>
    <Presentation />
    <Specialties />
    <Treatments />
    <TreatmentSurgicalOrthopedic />
    <CallToReserve 
      title="¡RESERVA TU CITA HOY!"
      subTitle="¿Quieres reservar una cita con nosotros?... Llámanos con toda confianza. Estamos aquí para ti."
      btnText="LLÁMANOS"
    />
  </div>
</template>

<script>
import Presentation from '@/components/present.vue';
import Specialties from "../components/specialties";
import Treatments from "../components/treatments.vue";
import TreatmentSurgicalOrthopedic from "../components/treatment-surgical-orthopedic.vue";
import CallToReserve from '@/components/call-to-reserve.vue';

export default {
  name: "Services",
  components:{
    Presentation,
    Specialties,
    Treatments,
    CallToReserve,
    TreatmentSurgicalOrthopedic
  }
}
</script>

<style scoped>

</style>