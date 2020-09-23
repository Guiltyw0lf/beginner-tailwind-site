<template>
  <div
    class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform shadow flex flex-col mb-8 rounded-lg"
  >
    <div
      class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
    >
      <h3 class="text-lg">{{ card_head }}</h3>
      <div class="flex space-x-2">
        <div class="w-3 h-3 rounded-full bg-red-500"></div>
        <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
        <div class="w-3 h-3 rounded-full bg-green-500"></div>
      </div>
    </div>
    <div class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0">
      <p>
        {{ card_body }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["card_head", "card_body"],
};
</script>