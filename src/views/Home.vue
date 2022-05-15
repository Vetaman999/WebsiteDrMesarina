<template>
  <div class="home" >
    
    <Presentation></Presentation>
    <convention style="margin: 100px 0 200px 0;"></convention>
    <Service style="margin: 100px 0 200px 0;"></Service>
    <Contact style="margin: 100px 0 200px 0;"></Contact>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Presentation from '@/components/present.vue'
import Service from '@/components/service.vue'
import Contact from '@/components/contact.vue'
import Convention from '@/components/convention.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Presentation,
    Service,
    Contact,
    Service,
    Convention
  }
}
</script>
