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
  <div>
    <product-card />
  </div>
</template>

<style lang="scss">
@import "@/assets/styles/app.scss";
</style>
