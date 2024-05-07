<script setup lang="ts">
const route = useRoute()
import burgers from '~/data/burgers.json'

</script>

<template>
  <div>
    <MainTitle title="Nos Burgers"/>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
      <CategoryCard
          v-for="burger in burgers"
          :key="burger.id"
          :category="burger"
          :title="burger.name"
          :description="burger.dsc"
          :image="burger.img"
          :price="burger.price"
      />
    </div>
  </div>
</template>

<style scoped>

</style>