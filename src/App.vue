<template>
  <div id="nav">
    <div>
      <Header :nav="links" />
    </div>
  </div>
  <router-view />
</template>
<script>
import Header from "@/components/nav/Header.vue";
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
  },
};
</script>
<style></style>
