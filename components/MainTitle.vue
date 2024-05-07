<script setup lang="ts">
const props = defineProps({
  title: String,
})
</script>

<template>
  <h2 class="bg-red-700 text-white text-center text-4xl p-8 mb-2 font-bold">{{title}}</h2>
</template>

<style scoped>

</style>