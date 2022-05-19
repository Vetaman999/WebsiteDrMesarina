<template>
  <div>
    <Presentation />
    <Specialties />
    <Treatments />
  </div>
</template>

<script>
import Presentation from "../components/present";
import Specialties from "../components/specialties";
import Treatments from "../components/treatments";

export default {
  name: "Services",
  components:{
    Presentation,
    Specialties,
    Treatments
  }
}
</script>

<style scoped>

</style>