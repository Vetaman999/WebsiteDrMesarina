<template>
  <div>
    <Presentation></Presentation>
    <CardProfile style="margin: 50px 0 50px 0;"></CardProfile>
    <our-mission></our-mission>
  </div>
</template>
<script> 
import Presentation from '@/components/present.vue'
import CardProfile from '@/components/card-profile.vue'
import OurMission from '@/components/our-mission.vue'

export default {
  name: 'Profile',
  components: {
    Presentation,
    CardProfile,
    OurMission
  }
}
</script>
