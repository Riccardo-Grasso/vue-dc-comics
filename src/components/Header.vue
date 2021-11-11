<template>
  <header>
    <div class="navbar-logo">
      <img src="../assets/dc-logo.png" alt="DC_Logo" />
    </div>

    <div class="navbar">
      <ul>
        <li class="navbar-item" v-for="(item, i) in navbarLinks" :key="i">
          <a :href="item.href">{{ item.title }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      navbarLinks: [
        {
          title: "CHARACTERS",
          href: "#",
        },
        {
          title: "COMICS",
          href: "#",
        },
        {
          title: "MOVIES",
          href: "#",
        },
        {
          title: "TV",
          href: "#",
        },
        {
          title: "GAMES",
          href: "#",
        },
        {
          title: "COLLECTIBLES",
          href: "#",
        },
        {
          title: "VIDEOS",
          href: "#",
        },
        {
          title: "FANS",
          href: "#",
        },
        {
          title: "NEWS",
          href: "#",
        },
        {
          title: "SHOP",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>
