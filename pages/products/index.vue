<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="p in products" :key="p.id">
        <ProductCard :product="p" />
      </div>
    </div>
  </div>
</template>

<script setup>
  const { data: products } = await useFetch('https://fakestoreapi.com/products')

  definePageMeta({
    layout: "products ",
  })
  useHead({
    title:'Nuxt Dojo for you | Merch',
    meta:[
      {name:'description',content:'Nuxt 3 mearch'}
    ]
  })
</script>