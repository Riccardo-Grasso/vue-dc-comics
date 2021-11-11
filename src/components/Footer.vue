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

    <div class="social">
      <div class="sign-up-button">
        <a href="#">SIGN-UP NOW!</a>
      </div>
      <div class="social-container">
        <div class="follow-us">FOLLOW US</div>
        <div class="social-list-container">
          <ul>
            <li class="social-icon" v-for="(social, i) in socialIcons" :key="i">
              <a href="#">
                <img :src="social.src" :alt="social.alt" />
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
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
      socialIcons: [
        {
          src: require("../assets/footer-facebook.png"),
          alt: "facebook",
        },
        {
          src: require("../assets/footer-twitter.png"),
          alt: "facebook",
        },
        {
          src: require("../assets/footer-youtube.png"),
          alt: "facebook",
        },
        {
          src: require("../assets/footer-pinterest.png"),
          alt: "facebook",
        },
        {
          src: require("../assets/footer-periscope.png"),
          alt: "facebook",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>
