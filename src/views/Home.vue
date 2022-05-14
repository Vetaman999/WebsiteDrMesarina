<template>
  <div class="home">
    
    <Presentation></Presentation>
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
    Presentation
  }
}
</script>
