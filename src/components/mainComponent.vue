<template>
  <main id="site_main">
    <jumbotronComponent/>
    <fumettiSectionComponent/>
    <secondaryMenu />
  </main>
</template>


<script>
import secondaryMenu from "@/components/secondaryMenuComponent.vue";
import jumbotronComponent from '@/components/jumbotronComponent.vue';
import fumettiSectionComponent from '@/components/fumettiSectionComponent.vue'

export default {
  name: "mainComponent",
  components: {
    secondaryMenu,
    jumbotronComponent,
    fumettiSectionComponent
  },
  
};
</script>
