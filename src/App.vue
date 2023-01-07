<script>
import ProductCard from "@/components/ProductCard.vue";
export default {
  name: "App",
  components: {
    ProductCard,
  },
};
</script>

<template>
  <main role="main">
    <product-card />
  </main>
</template>

<style lang="scss">
@import "@/assets/styles/app.scss";
</style>
