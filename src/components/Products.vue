<template>
  <div class="comic-container">
    <div class="img-container">
      <img :src="img" alt="product-image" />
    </div>
    <h4 class="comic-title">{{ title }}</h4>
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