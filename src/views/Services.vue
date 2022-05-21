<template>
  <div>
    <Separator separate="ESPECIALIDADES"/>
    <Specialties />
    <Separator separate="TRATAMIENTOS"/>
    <Treatments />
    <TreatmentSurgicalOrthopedic />
    <CallToReserve  style="margin: 50px 0 50px 0;"
      title="¡RESERVA TU CITA HOY!"
      subTitle="¿Quieres reservar una cita con nosotros?... Llámanos con toda confianza. Estamos aquí para ti."
      btnText="LLÁMANOS"
    />
  </div>
</template>

<script>
import Specialties from "../components/specialties";
import Treatments from "../components/treatments.vue";
import TreatmentSurgicalOrthopedic from "../components/treatment-surgical-orthopedic.vue";
import CallToReserve from '@/components/call-to-reserve.vue';
import Separator from '@/components/separator.vue'

export default {
  name: "Services",
  components:{
    Specialties,
    Treatments,
    CallToReserve,
    TreatmentSurgicalOrthopedic,
    Separator,
  }
}
</script>

<style scoped>

</style>