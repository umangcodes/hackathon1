<template>
  <div class="flex p-5 justify-between">
    <!-- Site logo -->
    <div>
      <h1>Logo</h1>
    </div>
    <!-- links -->
    <div class="flex">
      <div v-for="link in nav" :key="link.id" class="px-5">
        <router-link :to="link.url">{{ link.title }}</router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["nav"],
};
</script>

<style></style>
