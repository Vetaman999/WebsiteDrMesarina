<template>
  <div class="home">
    
    <AboutUs></AboutUs>
    <Presentation></Presentation>
    <Contact style="margin: 100px 0 200px 0;"></Contact>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Presentation from '@/components/service.vue'
import Contact from "@/components/contact";
import AboutUs from "@/components/about-us";

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Presentation,
    Contact,
    AboutUs
}
}
</script>
