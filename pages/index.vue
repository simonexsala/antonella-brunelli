<template>
  <main class="container flex-1 max-w-3xl px-6 mx-auto space-y-6 md:space-y-12 xl:max-w-5xl">
    <Hero />
    <Overview />
  </main>
</template>

<script setup>
const title = ref('Home / Antonella Brunelli')
const description = ref('Antonella Brunelli Irlanda con una Guida')
useHead({
  title,
  meta: [
    {
      name: 'description',
      content: description
    },
  ]
})
</script>
