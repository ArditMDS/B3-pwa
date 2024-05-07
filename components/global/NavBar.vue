<script setup lang="ts">

</script>

<template>
  <nav class="flex justify-between bg-red-700 p-5">
    <NuxtLink to="/">
      <Icon name="simple-icons:burgerking" color="white" size="50px"/>
    </NuxtLink>
    <div>
      <NuxtLink to="/cart">
        <Icon name="material-symbols:shopping-basket"  class="mr-3" color="white" size="50px"/>
      </NuxtLink>
      <Icon class="cursor-pointer" name="emojione:hamburger" color="black" size="50px"/>
    </div>
  </nav>
</template>

<style scoped>


</style>