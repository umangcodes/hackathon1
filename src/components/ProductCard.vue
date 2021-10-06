<template>
  <!-- <div :class="data.disable ? 'opacity-0'  : ''"> -->
  <div :class="data.disable ? 'opacity-30 hover:opacity-80' : ''">
    <div>
      <span class="text-xl font-bold">Serial #{{ data.id }}</span>
    </div>
    <div class="object-cover md:object-scale-down">
      <img src="https://tailwindcss.com/img/placeholder-amber.svg" alt="NA" />
    </div>
    <div class="">
      <span class="font-thin">Name </span>
      <br />
      <span class="font-thin">Power</span>
    </div>
    <span v-if="data.disable">Locked</span>
  </div>
  <!-- </div> -->
</template>

<script>
export default {
  props: ["data"],
};
</script>

<style></style>
