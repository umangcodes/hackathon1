<template>
  <div class="m-5">
    <div class="mb-16">
      <span class="text-2xl font-light border-b">Our Range</span>
    </div>
    <div class="grid grid-cols-1 xl:grid-cols-8 lg:grid-cols-6 md:grid-cols-3">
      <div v-for="product in products" :key="product.id">
        <div>
          <ProductCard :data="product" />
        </div>
      </div>
    </div>
    <button
      class="border-2 rounded-full px-2 py-1 text-lg bg-gray-200 text-gray-700"
      :onclick="buttonClick"
    >
      Load More
    </button>
  </div>
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
          disable: false,
        },
        {
          img: "xyz",
          id: 2,
          disable: false,
        },
        {
          img: "asdf",
          id: 3,
          disable: false,
        },
        {
          img: "abcd",
          id: 4,
          disable: false,
        },
        {
          img: "xyz",
          id: 5,
          disable: false,
        },
        {
          img: "asdf",
          id: 6,
          disable: false,
        },
        {
          img: "abcd",
          id: 7,
          disable: false,
        },
        {
          img: "xyz",
          id: 8,
          disable: true,
        },
        {
          img: "asdf",
          id: 9,
          disable: true,
        },
        {
          img: "xyz",
          id: 8,
          disable: true,
        },
        {
          img: "asdf",
          id: 9,
          disable: true,
        },
        {
          img: "xyz",
          id: 8,
          disable: true,
        },
        {
          img: "asdf",
          id: 9,
          disable: true,
        },
        {
          img: "xyz",
          id: 8,
          disable: true,
        },
        {
          img: "asdf",
          id: 9,
          disable: true,
        },
        {
          img: "xyz",
          id: 8,
          disable: true,
        },
        {
          img: "asdf",
          id: 9,
          disable: true,
        },
        {
          img: "xyz",
          id: 8,
          disable: true,
        },
        {
          img: "asdf",
          id: 9,
          disable: true,
        },
        {
          img: "xyz",
          id: 8,
          disable: true,
        },
        {
          img: "asdf",
          id: 9,
          disable: true,
        },
      ],
    };
  },
  components: {
    ProductCard,
  },
  methods: {
    buttonClick() {
      console.log("button pressed");
      // this.$router.push("/");
    },
  },
};
</script>

<style></style>
