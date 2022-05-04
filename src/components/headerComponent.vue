<template>
  <header id="site_header">
    <div class="container">
      <div class="row">
        <div class="col-4">
          <img src="@/assets/img/dc-logo.png" alt="" />
        </div>
        <div class="col-8">
          <nav>
            <a href="item.href" v-for="item in mainMenu" :key="item.id" :class="item.text === 'COMICS' ? 'active' : ''">
              {{ item.text }}
            </a>
          </nav>
        </div>
      </div>
    </div>
  </header>
</template>


<script>
export default {
  name: "headerComponent",
  data() {
    return {
      mainMenu: [
        {
          id: 1,
          href: "#",
          text: "CHARACTERS",
        },
        {
          id: 2,
          href: "#",
          text: "COMICS",
        },
        {
          id: 3,
          href: "#",
          text: "MOVIES",
        },
        {
          id: 4,
          href: "#",
          text: "TV",
        },
        {
          id: 5,
          href: "#",
          text: "GAMES",
        },
        {
          id: 6,
          href: "#",
          text: "COLLECTIBLES",
        },
        {
          id: 7,
          href: "#",
          text: "VIDEOS",
        },
        {
          id: 8,
          href: "#",
          text: "FANS",
        },
        {
          id: 9,
          href: "#",
          text: "NEWS",
        },
        {
          id: 10,
          href: "#",
          text: "SHOP",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#site_header {
  margin: 1rem 0;
  padding: 0.1rem;

  img {
    height: 80px;
  }

  a {
    text-decoration: none;
    padding: 2.5rem 0rem;
    font-size: 14px;
    font-weight: 700;
    color: #464646;
    margin: 0 0.75rem;

    &:hover, &.active {
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