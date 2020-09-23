<template>
  <div class="flex-grow p-10">
    <a class="text-2xl">{{ text }}</a>
  </div>
</template>

<script>
export default {
  props: ["text"],
};
</script>