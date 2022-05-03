<template>
  <div id="app">
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&display=swap"
      rel="stylesheet"
    />
    <siteHeader />
    <!-- /#site_header -->
    <siteMain/>
    <!-- /#site_main -->
    <siteFooter/>
    <!-- /#site_footer -->
  </div>
</template>

<script>
import siteHeader from "./components/headerComponent.vue";
import siteMain from "./components/mainComponent.vue";
import siteFooter from "./components/footerComponent.vue";

export default {
  name: "App",
  components: {
    siteHeader,
    siteMain,
    siteFooter
  },
};
</script>

<style lang="scss">
#app {
  font-family: "Lato", sans-serif;
}

/* style*/

@import '@/assets/sass/style';

/* grid system */

@import "@/assets/sass/_grid_system.scss";


</style>
