<template>
  <div id="app">
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&display=swap"
      rel="stylesheet"/>
    <siteHeader/>
    <!-- /#site_header -->
    <main id="site_main"></main>
    <!-- /#site_main -->
    <footer id="site_footer"></footer>
    <!-- /#site_footer -->
  </div>
</template>

<script>
import siteHeader from './components/headerComponent.vue'

export default {
  name: "App",
  components: {
    siteHeader
  },
};
</script>

<style lang="scss">
#app {
  font-family: 'Lato', sans-serif;
}

/* common rules */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  max-width: 100%;
}

/* importazioni */

@import "@/assets/sass/_grid_system.scss";
</style>
