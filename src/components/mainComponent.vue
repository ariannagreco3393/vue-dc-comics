<template>
  <main id="site_main">
    <section class="first_main_section">
      <div class="container">
        <div class="row">content goes here</div>
      </div>
    </section>
    <section class="secondary_menu">
      <div class="container">
        <div class="row">
            <div class="col-2" v-for="({src, titolo}, index) in secondaryMenu" :key="index">
                <a class="wrapper">
                    <img :src="src" :alt="titolo">
                    <h5>{{titolo}}</h5>
                </a>
            </div>
        </div>
      </div>
    </section>
  </main>
</template>


<script>
export default {
    name: 'mainComponent',
    data() {
       return {
           secondaryMenu: [
               {
                   src:'@/assets/img/buy-comics-digital-comics.png',
                   titolo: 'DIGITAL COMICS'
               },
               {
                   src:'@/assets/img/buy-comics-merchandise.png',
                   titolo: 'DC MERCHINDISE'
               },
               {
                   src:'@/assets/img/buy-comics-subscriptions.png',
                   titolo: 'SUBSCRIPTION'
               },
               {
                   src:'@/assets/img/buy-comics-shop-locator.png',
                   titolo: 'COMIC SHOP LOCATOR'
               },
               {
                   src:'@/assets/img/buy-comics-dc-power-visa.svg',
                   titolo: 'DC POWER VISA'
               }
           ]
       } 
    }
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

  .secondary_menu {
    height: 130px;
    width: 100%;
    background-color: rgb(0, 130, 249);
  }
}
</style>