<template>
  <div>
    <h2 class=" ">About</h2>
    <p>Lorem ipsum dolor  sit amet consectetur adipisicing. Eveniet aperiam minima unde nemo harum quam maxime optio quos corrupti. Eum sapiente facere nemo, laborum ullam non cum fuga quas eveniet harum molestiae minus atque vel ratione illo quia, iure commodi dicta porro excepturi quam. Facere, commodi corrupti ipsam neque totam reprehenderit laboriosam laborum veniam est quo, repellat saepe impedit labore?</p>
    <p>api response here:</p>
    <div>{{ data }}</div>
  </div>
</template>

<style scoped>
  h2 {
    margin-bottom: 20px;
    font-size: 36px;
  }
  p {
    margin: 20px ;
  
  }
</style>

<script setup>
 

  const { data } = await useFetch('/api/currency/GBP')
</script>