<template>
  <footer id="site_footer">
    <footerTopComponent/>
    <footerBottomComponent/>
  </footer>
</template>

<script>
import footerTopComponent from '@/components/footerTopComponent.vue'
import footerBottomComponent from '@/components/footerBottomComponent.vue'

export default {
  name: "footerComponent",
  components: {
      footerTopComponent,
      footerBottomComponent
  }
};
</script>
