<script setup lang="ts">
import desserts from "~/data/desserts.json";
</script>

<template>
  <div>
    <MainTitle title="Nos Desserts"/>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
      <CategoryCard
          v-for="dessert in desserts"
          :key="dessert.id"
          :category="dessert"
          :title="dessert.name"
          :description="dessert.dsc"
          :image="dessert.img"
          :price="dessert.price"
      />
    </div>
  </div>

</template>

<style scoped>

</style>