<script setup lang="ts">
import Button from '@/components/ui/button/Button.vue'

import { ShieldCheck, NotebookPen } from 'lucide-vue-next'

const checks = [
  {
    index: 1,
    description: '100% Satisfaction Guaranteed'
  },
  {
    index: 2,
    description: 'Qualityful Instrument'
  },
  {
    index: 3,
    description: 'Expert Cleaning Team'
  },
  {
    index: 4,
    description: '24/7 Online Support'
  }
]
</script>

<template>
  <div>
    <div class="mx-auto flex flex-col xl:flex-row 2xl:max-w-[1440px]">
      <!-- LEFT SECTION -->
      <div class="xl:w-1/3">
        <img class="rounded-xl object-cover" src="../assets/img/about-us-one.jpeg" alt="" />
        <div class="mt-4 flex gap-2.5">
          <span class="font-body text-6xl font-bold text-primary">35</span>
          <p class="font-title text-xl font-bold">Years <br />Experience</p>
        </div>
      </div>

      <!-- RIGHT SECTION -->
      <div class="grid place-items-center text-center xl:w-2/3 xl:place-items-start xl:text-start">
        <span class="flex items-end gap-3 text-xl font-medium text-subtitle">
          <img class="mb-1.5 w-7" src="../assets/img/broom-icon.svg" alt="Broom Icon" />ABOUT
          COMPANY
        </span>

        <h1 class="mt-5 text-3xl font-bold sm:mt-6 sm:text-4xl sm:leading-[50px] xl:text-5xl">
          Our Promise Is To Deliver Only The Best
          <span class="font-title text-primary">Services</span>
        </h1>

        <p class="text-description mt-6 font-light leading-7 tracking-wide">
          For over a decade, our cleaning service company an beacon of cleanliness and
          professionalism We take pride in providing top-tier cleaning solutions to businesses,
          ensuring their spaces are pristine, healthy, and inviting for employees.
        </p>

        <div class="mt-8 grid gap-2 gap-x-10 sm:grid-cols-2 md:gap-y-4 xl:gap-2.5">
          <div v-for="check in checks" :key="check.index" class="flex items-center">
            <ShieldCheck class="mr-2 h-8 w-8 fill-primary stroke-white" />
            <p class="font-medium tracking-wide">{{ check.description }}</p>
          </div>
        </div>

        <Button class="mt-8 h-14 px-6"><NotebookPen class="mr-1.5 w-5" />Angebot anfordern</Button>
      </div>
    </div>
  </div>
</template>
