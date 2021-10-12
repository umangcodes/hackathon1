<template>
  <div class="h-screen relative border">
    <div class="">
      <h1>Home Page</h1>
    </div>
    <div class="">
      <!-- relative bottom-0 -->
      <Tech />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Tech from "@/components/WelcomeComponents/Tech.vue";
export default {
  name: "Home",
  components: {
    Tech,
  },
};
</script>
