<template>
  <div>
    <div class="flex bg-gray-200 rounded shadow">
      <div
        class="w-1/3 flex items-center text-center justify-center uppercase font-bold rounded-l text-3xl"
        v-bind:style="[baseStyles]"
      > 😍</div>
      <div class="flex-grow p-4">{{ button }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["button", "baseStyles"],
};
</script>