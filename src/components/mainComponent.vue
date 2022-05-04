<template>
  <main id="site_main">
    <section class="jumbotron">
      <div class="container">
        <div class="label">
          <p>CURRENT SERIES</p>
        </div>
      </div>
    </section>
    <section class="first_main_section">
      <div class="container">
        <div class="row"></div>
      </div>
    </section>
    <secondaryMenu />
  </main>
</template>


<script>
import secondaryMenu from "@/components/secondaryMenuComponent.vue";
export default {
  name: "mainComponent",
  components: {
    secondaryMenu,
  },
};
</script>

<style lang="scss" scoped>
/* main */

#site_main {
  .jumbotron {
    height: 300px;
    background-image: url("@/assets/img/jumbotron.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    img {
      max-width: 100%;
    }

    .label {
      background-color: rgb(0, 130, 249);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 30px;
      width: 10%;
      position: absolute;
      bottom: -1rem;
      
      p {
        color: white;
        font-weight: 700;
      }
    }
  }
}

#site_main {
  .first_main_section {
    width: 100%;
    height: 100px;
    background-color: #1c1c1c;
    color: white;
  }
}
</style>