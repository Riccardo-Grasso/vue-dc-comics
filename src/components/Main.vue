<template>
  <main class="content-container">
    <div class="jumbotron">
      <img src="@/assets/jumbotron.jpg" alt="jumbo-img" />
    </div>
    <div class="comics-container">
      <Products
        v-for="(p, i) in comicsList"
        :key="i"
        :img="p.thumb"
        :title="p.series"
        :price="p.price"
        :type="p.type"
      ></Products>
    </div>
  </main>
</template>

<script>
import Products from "../components/Products.vue";
import jsonData from "../database/dc-comics.json";

export default {
  name: "Main",
  components: {
    Products,
  },
  data() {
    return {
      comicsList: jsonData,
    };
  },
};
</script>

<style scoped>
</style>
