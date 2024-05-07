<script setup lang="ts">
const props = defineProps({
  category: String,
  title: String,
  description: String,
  image: String,
  price: Number
})

const cart = useState('cart', () => [])

function addToCart() {
  cart.value.push(props)
}
</script>

<template>
  <div class="bg-white rounded-lg shadow-lg overflow-hidden">
    <img :src="image" alt="burger" class="w-full h-64 object-cover object-center">
    <div class="p-4">
      <h3 class="text-xl font-bold">{{title}}</h3>
      <p class="text-gray-600">{{description}}</p>
      <p class="text-red-700 font-bold text-xl">{{price}} €</p>
      <button @click="addToCart" class="block mt-4 bg-red-700 text-white text-center text-lg p-2 rounded-lg">Acheter</button>
    </div>
  </div>

</template>

<style scoped>

</style>