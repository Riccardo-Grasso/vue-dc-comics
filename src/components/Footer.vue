<template>
  <footer>
    <div class="footer-icons-container">
      <ul>
        <li class="footer-icons" v-for="(icon, i) in footerIcons" :key="i">
          <a :href="icon.href">
            <img :src="icon.img" :alt="icon.alt" />
            <div class="icon-text">{{ icon.text }}</div>
          </a>
        </li>
      </ul>
    </div>

    <div class="footer-list-container">fdgdfg</div>

    <div class="social"></div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      footerIcons: [
        {
          img: require("../assets/buy-comics-digital-comics.png"),
          alt: "icon",
          text: "DIGITAL COMICS",
          href: "#",
        },
        {
          img: require("../assets/buy-comics-merchandise.png"),
          alt: "icon",
          text: "DC MERCHANDISE",
          href: "#",
        },
        {
          img: require("../assets/buy-comics-subscriptions.png"),
          alt: "icon",
          text: "SUBSCRIPTION",
          href: "#",
        },
        {
          img: require("../assets/buy-comics-shop-locator.png"),
          alt: "icon",
          text: "COMIC SHOP LOCATOR",
          href: "#",
        },
        {
          img: require("../assets/buy-dc-power-visa.svg"),
          alt: "icon",
          text: "DC POWER VISA",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>
