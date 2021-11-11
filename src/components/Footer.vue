<template>
  <footer>
    <div class="footer-icons-container">
      <ul>
        <li class="footer-icons" v-for="(icon, i) in footerIcons" :key="i">
          <a :href="icon.href">
            <img :src="icon.img" :alt="icon.alt" />
            <div>{{ icon.text }}</div>
          </a>
        </li>
      </ul>
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
          img: "../assets/buy-comics-digital-comics.png",
          alt: "icon",
          text: "DIGITAL COMICS",
          href: "#",
        },
        {
          img: "../assets/buy-comics-digital-comics.png",
          alt: "icon",
          text: "DC MERCHANDISE",
          href: "#",
        },
        {
          img: "../assets/buy-comics-digital-comics.png",
          alt: "icon",
          text: "DIGITAL COMICS",
          href: "#",
        },
        {
          img: "../assets/buy-comics-digital-comics.png",
          alt: "icon",
          text: "DIGITAL COMICS",
          href: "#",
        },
        {
          img: "../assets/buy-comics-digital-comics.png",
          alt: "icon",
          text: "DIGITAL COMICS",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>
