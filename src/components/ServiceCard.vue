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
  <div class="w-[410px] overflow-hidden rounded-xl pb-4 shadow-md">
    <img class="w-full object-cover" :src="image" alt="Card image" />

    <div class="relative grid place-items-center px-6 py-4 text-center">
      <div class="rhombus absolute -top-11 flex w-56 justify-center bg-white py-6">
        <Warehouse class="h-10 w-10 stroke-1" />
      </div>

      <h3 class="mt-8 text-2xl font-bold">{{ title }}</h3>
      <p class="text-description mt-3.5 font-light leading-7">
        {{ description }}
      </p>
      <Button class="mt-6 h-11 px-8">See More<ArrowUpRight class="ml-1.5 h-5 w-5" /></Button>
    </div>
  </div>
</template>

<style>
.rhombus {
  clip-path: polygon(50% 0, 100% 50%, 50% 100%, 0% 50%);
}
</style>
