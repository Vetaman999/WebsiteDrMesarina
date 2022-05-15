<template>
  <div class="home">
    
    <Presentation></Presentation>
    <Contact style="margin: 100px 0 200px 0;"></Contact>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Presentation from '@/components/service.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Presentation,
    Contact
}
}
</script>
