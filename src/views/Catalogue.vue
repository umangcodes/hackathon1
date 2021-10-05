<template>
  <ProductCard v-for="product in products" :data="product" :key="product.id" />
</template>

<script>
import ProductCard from "@/components/ProductCard.vue";
export default {
  data() {
    return {
      products: [
        {
          img: "abcd",
          id: 1,
        },
        {
          img: "xyz",
          id: 2,
        },
        {
          img: "asdf",
          id: 3,
        },
      ],
    };
  },
  components: {
    ProductCard,
  },
};
</script>

<style></style>
