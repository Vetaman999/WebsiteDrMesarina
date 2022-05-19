<template>
  <div>
    <Presentation />
    <Separator separate="ACTUALIZACIONES"/>
    
    <Galery></Galery>
    <Fb />
  </div>
</template>

<script>
import Presentation from '@/components/present.vue';
import Fb from '@/components/fb.vue';
import Separator from '@/components/separator.vue';
import Galery from '@/components/galery.vue'

export default {
  name: "Update",
  components:{
    Presentation,
    Fb,
    Separator,
    Galery,
  }
}
</script>

<style scoped>

</style>