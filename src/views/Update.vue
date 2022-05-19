<template>
  <div>
    <Presentation />
    <Fb />
  </div>
</template>

<script>
import Presentation from '@/components/present.vue';
import Fb from '@/components/fb.vue';


export default {
  name: "Update",
  components:{
    Presentation,
    Fb,
  }
}
</script>

<style scoped>

</style>