<template>
  <div
    class="flex-grow bg-orange-900 my-8 p-12 hover:bg-orange-600 md:rounded-r-lg"
  >
    <a class="text-2xl">{{ text }}</a>
  </div>
</template>

<script>
export default {
  props: ["text"],
};
</script>