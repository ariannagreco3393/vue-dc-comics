<template>
  <header id="site_header">
    <div class="container">
      <div class="row">
        <div class="col-4">
          <img src="@/assets/img/dc-logo.png" alt="" />
        </div>
        <div class="col-8">
          <nav>
            <a href="#" v-for="(voce, index) in mainMenu" :key="index">{{voce}}</a>
          </nav>
        </div>
      </div>
    </div>
  </header>
</template>


<script>
export default {
    name: 'headerComponent',
    data() {
        return {
            mainMenu: ['CHARACTERS', 'COMICS', 'MOVIES', 'TV', 'GAMES', 'COLLECTIBLES', 
            'VIDEOS', 'FANS', 'NEWS', 'SHOP']
        }
    }
    
}
</script>

<style lang="scss" scoped>
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
      color: rgb(0, 130, 249);
      border-bottom: 4px solid rgb(0, 130, 249);
    }
  }
  .col-8 {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>