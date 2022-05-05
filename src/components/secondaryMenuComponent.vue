<template>
    <section class="secondary_menu">
      <div class="container">
        <div class="row">
            <div class="col" v-for="({src, text}, index) in secondaryMenu" :key="index">
                <a class="wrapper">
                    <img :src="src">
                    <span>{{text}}</span>
                </a>
            </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    name: 'secondaryMenu',
    data() {
       return {
           secondaryMenu: [
               {
                   src: require("@/assets/img/buy-comics-digital-comics.png"),
                   text: 'DIGITAL COMICS'
               },
               {
                   src:require("@/assets/img/buy-comics-merchandise.png"),
                   text: 'DC MERCHINDISE'
               },
               {
                   src: require("@/assets/img/buy-comics-subscriptions.png"),
                   text: 'SUBSCRIPTION'
               },
               {
                   src:require("@/assets/img/buy-comics-shop-locator.png"),
                   text: 'COMIC SHOP LOCATOR'
               },
               {
                   src:require("@/assets/img/buy-dc-power-visa.svg"),
                   text: 'DC POWER VISA'
               }
           ]
       } 
    }
}
</script>

<style lang="scss" scoped>
    .secondary_menu {
    width: 100%;
    background-color: $dc-primary;
    padding: 2rem;

    .wrapper{
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 12px;
        color: $white;
        
    }
    img {
        max-width: 100%;
        height: 40px;
        margin-right: 1rem;
    }
  }
</style>