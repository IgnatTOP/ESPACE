<template>
 <div ref="a1" class="a111"><Header_Component @scroll2="scrollToOpisanie" @scroll4="scrollTodownload"/></div>
 <div ref="a2" class="a111"><Content_Component/></div>
 <div ref="a3" class="a111"><Trailer_Component/></div>
 <div ref="a4" class="a111"><Download_Component/></div>
</template>
<script>
import Header_Component from "@/components/Header_component.vue";
import Content_Component from "@/components/Content_component.vue";
import Trailer_Component from "@/components/Trailer_component.vue";
import Download_Component from "@/components/Download_component.vue";

export default {
    name: 'Home_Component',
    components: {
     Download_Component,
     Trailer_Component,
     Content_Component,
        Header_Component
    },
 methods: {
  scrollToOpisanie() {
   this.$refs.a2.scrollIntoView({ behavior: 'smooth' });
  },
  scrollTodownload() {
   this.$refs.a4.scrollIntoView({ behavior: 'smooth' });
  }
 }
}
</script>

<style scoped>
.a111{
 height: auto;
}
</style>