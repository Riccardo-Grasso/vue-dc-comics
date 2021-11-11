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

    <div class="footer-list-container">
      <div class="link-container">
        <div class="col-1">
          <div class="col-top">
            <div class="title">DC COMICS</div>
            <ul>
              <li class="links" v-for="(element, i) in linkTop" :key="i">
                <a :href="element.href">{{ element.link }}</a>
              </li>
            </ul>
          </div>
          <div class="col-bottom">
            <div class="title">SHOP</div>
            <ul>
              <li class="links" v-for="(element, i) in linkBottom" :key="i">
                <a :href="element.href">{{ element.link }}</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-2">
          <div class="title">DC</div>
          <ul>
            <li class="links" v-for="(element, i) in linkCentral" :key="i">
              <a :href="element.href">{{ element.link }}</a>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <div class="title">SITES</div>
          <ul>
            <li class="links" v-for="(element, i) in linkRight" :key="i">
              <a :href="element.href">{{ element.link }}</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="image-container">
        <img src="../assets/dc-logo-bg.png" alt="logo-big" />
      </div>
    </div>

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
      linkTop: [
        { link: "Characters", href: "#" },
        { link: "Comics", href: "#" },
        { link: "Movies", href: "#" },
        { link: "TV", href: "#" },
        { link: "Games", href: "#" },
        { link: "Videos", href: "#" },
        { link: "News", href: "#" },
      ],
      linkBottom: [
        { link: "Shop DC", href: "#" },
        { link: "Shop DC Collectibles", href: "#" },
      ],
      linkCentral: [
        { link: "Terms Of Use", href: "#" },
        { link: "Privacy policy (New)", href: "#" },
        { link: "Ad Choices", href: "#" },
        { link: "Advertising", href: "#" },
        { link: "Jobs", href: "#" },
        { link: "Subscriptions", href: "#" },
        { link: "Talent Workshops", href: "#" },
        { link: "CPSC Certificates", href: "#" },
        { link: "Ratings", href: "#" },
        { link: "Shop Help", href: "#" },
        { link: "ontact Us", href: "#" },
      ],
      linkRight: [
        { link: "DC", href: "#" },
        { link: "MAD Magazine", href: "#" },
        { link: "DC Kids", href: "#" },
        { link: "DC Universe", href: "#" },
        { link: "DC Power Visa", href: "#" },
      ],
    };
  },
};
</script>

<style scoped>
</style>
