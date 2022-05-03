<template>
  <div id="app">
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&display=swap"
      rel="stylesheet"/>
    <header id="site_header">
      <div class="container">
        <div class="row">
          <div class="col-4">
            <img src="@/assets/img/dc-logo.png" alt="">
          </div>
          <div class="col-8">
            <nav>
              <a href="">CHARACTERS</a>
              <a href="" class="active">COMICS</a>
              <a href="">MOVIES</a>
              <a href="">TV</a>
              <a href="">GAMES</a>
              <a href="">COLLECTIBLES</a>
              <a href="">VIDEOS</a>
              <a href="">FANS</a>
              <a href="">NEWS</a>
              <a href="">SHOP</a>
            </nav>
          </div>
        </div>
      </div>
    </header>
    <!-- /#site_header -->
    <main id="site_main"></main>
    <!-- /#site_main -->
    <footer id="site_footer"></footer>
    <!-- /#site_footer -->
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style lang="scss">
#app {
  font-family: 'Lato', sans-serif;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


#site_header {
  height: 100px;
  margin: 1rem 0;

  img {
    height: 80px;
  }

  a {
    text-decoration: none;
    padding: 2.5rem 0rem;
    font-size: 14px;
    font-weight: 700;
    color: #464646;
    margin: 0 0.85rem;
  }

  nav {

    .active {
      color: rgb(0,130,249);
      border-bottom: 4px solid rgb(0,130,249);
    }
  }
  .col-8 {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}

/* common rules */
img {
  max-width: 100%;
}

@import "@/assets/sass/_grid_system.scss";
</style>
