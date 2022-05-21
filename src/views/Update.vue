<template>
  <div>
    <Separator separate="ACTUALIZACIONES"/>
    <Fb />
    <Galery></Galery>
    
  </div>
</template>

<script>
import Fb from '@/components/fb.vue';
import Separator from '@/components/separator.vue';
import Galery from '@/components/galery.vue'

export default {
  name: "Update",
  components:{
    Fb,
    Separator,
    Galery,
  }
}
</script>

<style scoped>

</style>