<template>
  <div class="text-center font-semibold grid grid-cols-3 gap-14 m-auto p-10 relative">
    <div v-for="p in products" class="">
      <div class="w-1/3 m-auto mb-5"><img :src="p.image" alt="product-image"></div>
      <div>
        <div class="object-bottom">{{ p.title }}</div>
        <div class="font-bold">{{ p.price }}</div>
        <div class="font-normal">{{ p.category }}</div>
      </div>
    </div>
  </div>
</template>

<script setup>

const { data: products } = await useFetch('https://fakestoreapi.com/products')

const { product } = defineProps(['p'])

</script>

<style scoped></style>