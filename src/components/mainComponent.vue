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
        <div class="row">
          <div class="col-2" v-for="(card, index) in cards" :key="index">
            <div class="card">
              <div class="img_card">
                <img :src="card.thumb" alt="" />
              </div>
              <div class="text_card">
                <p>{{ card.series }}</p>
              </div>
            </div>
          </div>
          <div class="btn">
            <a href="#">LOAD MORE</a>
          </div>
        </div>
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
  data() {
    return {
      cards: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
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
    padding: 2rem;
    width: 100%;
    background-color: #1c1c1c;
    color: white;
  }
  .card {
    padding: 0.75rem;

    .img_card {
      img {
        aspect-ratio: 1/1;
        object-fit: cover;
        object-position: top;
      }
    }

    .text_card {
      p {
        text-transform: uppercase;
        padding-top: 1rem;
      }
    }
  }

  .btn {
    width: 100%;
    padding: 2rem 1rem 0;
    display: flex;
    justify-content: center;
    a {
      text-decoration: none;
      background-color: rgb(0, 130, 249);
      padding: 0.8rem 3rem;
      color: white;
      font-size: 13px;
      font-weight: 700;
    }
  }
}
</style>