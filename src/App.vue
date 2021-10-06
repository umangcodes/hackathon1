<template>
  <div id="nav">
    <div class="static">
      <Header :nav="links" />
    </div>
  </div>
  <router-view />
  <Footer :nav="links" />
</template>
<script>
import Header from "@/components/nav/Header.vue";
import Footer from "@/components/nav/Footer.vue";
export default {
  data() {
    return {
      links: [
        { id: "91", title: "Home", url: "/" },
        { id: "92", title: "Catalogue", url: "/catalogue" },
        { id: "93", title: "About", url: "/about" },
      ],
    };
  },
  components: {
    Header,
    Footer,
  },
};
</script>
<style></style>
