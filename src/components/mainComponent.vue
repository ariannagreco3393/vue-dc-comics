<template>
  <main id="site_main">
    <section class="first_main_section">
      <div class="container">
        <div class="row">content goes here</div>
      </div>
    </section>
    <secondaryMenu/>
  </main>
</template>


<script>
import secondaryMenu from '@/components/secondaryMenuComponent.vue'
export default {
    name: 'mainComponent',
    components: {
        secondaryMenu
    },
   
}
</script>

<style lang="scss" scoped>
/* main */

#site_main {
  .first_main_section {
    width: 100%;
    height: 100px;
    background-color: #1c1c1c;
    color: white;
  }
}
</style>