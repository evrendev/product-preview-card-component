<template>
  <div class="container">
    <div class="card bg-primary-100">
      <div class="product-image">
        <img src="@/assets/images/image-product-desktop.jpg" alt="Product Image" />
      </div>
      <div class="product-info">
        <div>
          <span class="product-category text-neutral-900"> Perfume </span>
        </div>
        <div>
          <h2 class="product-title ff-heading fw-bold fs-900">Gabrielle Essence Eau De Parfum</h2>
        </div>
        <div>
          <p class="product-description text-neutral-900">
            A floral, solar and voluptuous interpretation composed by Olivier Polge,
            Perfumer-Creator for the House of CHANEL.
          </p>
        </div>
        <div class="price-wrapper">
          <span class="current-price ff-heading fs-900 text-primary-400 fw-regular"> $149.99 </span>
          <span class="old-price text-line-through text-neutral-900"> $169.99 </span>
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
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100vw;
  height: 100vh;

  .card {
    width: 50em;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0;
    border-radius: 1rem;
    box-shadow: 0 0 10px 0 var(--clr-neutral-100);
    overflow: hidden;

    .product-image {
      background-image: url("@/assets/images/image-product-desktop.jpg");
      background-position: top left;
      background-size: contain;
      background-repeat: no-repeat;

      img {
        visibility: hidden;
      }
    }

    .product-info {
      padding: 2em;

      > div {
        margin-bottom: 3em;
      }

      span {
        &.product-category {
          letter-spacing: 2px;
          text-transform: uppercase;
        }
      }

      .price-wrapper {
        display: flex;
        align-items: center;

        .old-price {
          margin-left: 2rem;
        }
      }

      button {
        &.add-to-cart {
          width: 100%;
          background-color: var(--clr-primary-400);
          color: var(--clr-primary-100);
          border: 0;
          border-radius: 0.5rem;
          padding: 1rem;
          display: inline-flex;
          align-items: center;
          justify-content: center;

          span {
            margin-left: 1rem;
          }
        }
      }
    }
  }
}
</style>
