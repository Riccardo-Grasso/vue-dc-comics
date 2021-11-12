<template>
  <div class="comic-container">
    <img :src="img" alt="product-image" />
    <h4>{{ title }}</h4>
  </div>
</template>

<script>
export default {
  name: "Products",
  props: ["img", "title"],
};
</script>

<style scoped>
</style>