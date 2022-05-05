<template>
  <div class="footer_top">
    <div class="container">
      <div class="row">
        <div class="col-6 menu">
          <div class="row">
            <div
              class="col-4"
              v-for="({ title, links }, index) in footerMenu"
              :key="index"
            >
              <h3>{{ title }}</h3>
              <ul>
                <li v-for="(link, index) in links" :key="index">
                  <a href="link.href">{{ link.text }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-6 bg_logo"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "footerTopComponent",
  data() {
    return {
      footerMenu: [
        {
          title: "DC COMICS",
          links: [
            {
              href: "#",
              text: "Characters",
            },
            {
              href: "#",
              text: "comics",
            },
            {
              href: "#",
              text: "Movies",
            },
            {
              href: "#",
              text: "Tv",
            },
            {
              href: "#",
              text: "Games",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "News",
            },
          ],
        },
        {
          title: "DC",
          links: [
            {
              href: "#",
              text: "terms of use",
            },
            {
              href: "#",
              text: "privacy policy",
            },
            {
              href: "#",
              text: "Ad Choices",
            },
            {
              href: "#",
              text: "Advertising",
            },
            {
              href: "#",
              text: "Jobs",
            },
            
          ],
        },
        {
          title: "SITES",
          links: [
            {
              href: "#",
              text: "dc",
            },
            {
              href: "#",
              text: "mad magazine",
            },
            {
              href: "#",
              text: "Dc kids",
            },
            {
              href: "#",
              text: "Dc universe",
            },
            {
              href: "#",
              text: "Dc power visa",
            },
          ],
        },
        {
          title: "SHOP",
          links: [
            {
              href: "#",
              text: "shop dc",
            },
            {
              href: "#",
              text: "lorem",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>

</style>