<template>
  <div class="container">
    <div class="card">
      <div class="product-image"></div>
      <div class="product-info">
        <span class="category"> Parfume </span>
        <h2 class="product-title">Gabrielle Essence Eau De</h2>
        <p class="product-description">
          A floral, solar and voluptuous interpretation composed by Olivier Polge, Perfumer-Creator
          for the House of CHANEL.
        </p>
        <div class="price-wrapper">
          <span class="current-price"> $149.99 </span>
          <span class="old-price"> $169.99 </span>
        </div>
        <button class="add-to-cart">
          <img src="@/assets/images/icon-cart.svg" alt="Add to Cart Icon" />
          <span> Add to Cart </span>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductCard",
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>
