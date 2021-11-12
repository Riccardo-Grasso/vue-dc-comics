<template>
  <main class="content-container">
    <Products
      v-for="(product, i) in comicsList"
      :key="i"
      :img="product.thumb"
      :title="product.series"
      :price="product.price"
      :type="product.type"
    ></Products>
  </main>
</template>

<script>
import jsonData from "../database/dc-comics.json";
import Products from "../components/Products.vue";

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
