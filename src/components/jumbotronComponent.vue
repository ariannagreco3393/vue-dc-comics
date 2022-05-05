<template>
    <section class="jumbotron">
      <div class="container">
        <div class="label">
          <p>CURRENT SERIES</p>
        </div>
      </div>
    </section> 
</template>

<script>
export default {
    name: 'jumbotronComponent'
}
</script>

<style lang="scss" scoped>
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
      background-color: $dc-primary;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 30px;
      width: 10%;
      position: absolute;
      bottom: -1rem;

      p {
        color: $white;
        font-weight: 700;
      }
    }
  }
}
</style>