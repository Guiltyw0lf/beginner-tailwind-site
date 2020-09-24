<template>
  <div class="border-2 border-gray-500 rounded-lg p-8 text-gray-200">
    <h3 class="font-bold text-xl mb-3">{{ faq_header }}</h3>
    <span> {{ faq_body }}</span>
    <span v-bind:style="[color1]"> {{ color1_text }} </span>
    <span v-bind:style="[color2]"> {{ color2_text }} </span>
  </div>
</template>

<script>
export default {
  props: [
    "faq_header",
    "faq_body",
    "color1",
    "color2",
    "color1_text",
    "color2_text",
  ],
};
</script>