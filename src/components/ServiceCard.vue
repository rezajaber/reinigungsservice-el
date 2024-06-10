<script setup>
import Button from '@/components/ui/button/Button.vue'

import { ArrowUpRight, Warehouse } from 'lucide-vue-next'

defineProps({
  image: String,
  title: String,
  description: String,
  link: String
})
</script>

<template>
  <div class="">
    <img src="../assets/img/service-card-one.jpeg" class="w-full object-cover" alt="Card image" />

    <div
      class="relative flex flex-grow flex-col items-center justify-between px-6 py-4 text-center"
    >
      <div class="rhombus absolute -top-11 flex w-56 justify-center bg-white py-6">
        <Warehouse class="h-10 w-10 stroke-primary stroke-1" />
      </div>

      <h3 class="mt-8 text-2xl font-bold">Titel der Wäsche</h3>
      <p class="mt-3.5 text-sm font-light leading-7 text-description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius, sed sint rerum ea voluptatum
        minus dolorum quam autem cumque commodi earum odio
      </p>
      <Button class="my-6 h-11 px-8">See More<ArrowUpRight class="ml-1.5 h-5 w-5" /></Button>
    </div>
  </div>
</template>

<style scoped>
.rhombus {
  clip-path: polygon(50% 0, 100% 50%, 50% 100%, 0% 50%);
}
</style>
