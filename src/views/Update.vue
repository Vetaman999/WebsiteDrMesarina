<template>
  <div>
    <Presentation />
    <Separator separate="ACTUALIZACIONES"/>
    <Fb />
  </div>
</template>

<script>
import Presentation from '@/components/present.vue';
import Fb from '@/components/fb.vue';
import Separator from '@/components/separator.vue';

export default {
  name: "Update",
  components:{
    Presentation,
    Fb,
    Separator,
  }
}
</script>

<style scoped>

</style>