<template>
  <div :class="data.disable ? 'opacity-30' : ''">
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
    <div class="opacity-0 hover:opacity-100" v-if="data.disable">Locked</div>
  </div>
</template>

<script>
export default {
  props: ["data"],
};
</script>

<style></style>
