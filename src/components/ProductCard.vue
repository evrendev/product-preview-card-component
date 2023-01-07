<template>
  <div class="container">
    <div class="card bg-primary-100">
      <div class="product-image">
        <img
          src="@/assets/images/image-product-desktop.jpg"
          alt="Gabrielle Essence Eau De Parfum"
        />
      </div>
      <div class="product-info">
        <div>
          <span class="product-category text-neutral-900"> Perfume </span>
        </div>
        <div>
          <h1 class="product-title ff-heading fw-bold fs-900">Gabrielle Essence Eau De Parfum</h1>
        </div>
        <div>
          <p class="product-description text-neutral-900">
            A floral, solar and voluptuous interpretation composed by Olivier Polge,
            Perfumer-Creator for the House of CHANEL.
          </p>
        </div>
        <div class="price-wrapper">
          <span class="current-price ff-heading fs-900 text-primary-400 fw-regular"> $149.99 </span>
          <del class="old-price text-line-through text-neutral-900 sr-only"> $169.99 </del>
        </div>
        <button class="add-to-cart">
          <svg-icon :name="'icon-cart'" />
          <span> Add to Cart </span>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import SvgIcon from "@/components/SvgIcon.vue";

export default {
  name: "ProductCard",
  components: {
    SvgIcon,
  },
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/styles/card.scss";
</style>
