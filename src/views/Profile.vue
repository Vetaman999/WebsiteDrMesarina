<template>
  <div>
    <CardProfile style="margin: 50px 0 50px 0;"></CardProfile>
    <Biography></Biography>
    <OurMission></OurMission>
    <ConsultingRoom></ConsultingRoom>
    <SpecializedServices></SpecializedServices>
    <GoOffice></GoOffice>
    <Contact style="margin: 50px 0 50px 0;"></Contact>
  </div>
</template>
<script> 
import CardProfile from '@/components/card-profile.vue'
import OurMission from '@/components/our-mission.vue'
import Biography from '@/components/biography.vue'
import ConsultingRoom from '@/components/consulting-room.vue'
import Contact from '@/components/contact.vue'
import SpecializedServices from '@/components/specialized-services.vue'
import GoOffice from '@/components/go-office.vue'
import Separator from '@/components/separator.vue'

export default {
  name: 'Profile',
  components: {
    CardProfile,
    OurMission,
    Biography,
    ConsultingRoom,
    Contact,
    SpecializedServices,
    GoOffice,
    Separator,
  }
}
</script>
