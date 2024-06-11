<script setup lang="ts">
import Button from '@/components/ui/button/Button.vue'

import { ShieldCheck, NotebookPen } from 'lucide-vue-next'

const checks = [
  {
    index: 1,
    description: '100% Zufriedenheitsgarantie'
  },
  {
    index: 2,
    description: 'Qualitätsvolle Instrumente'
  },
  {
    index: 3,
    description: 'Engagiertes Team'
  },
  {
    index: 4,
    description: 'Schneller Support'
  }
]

const scrollTo = (id: string) => {
  const element = document.getElementById(id)
  if (element) {
    const offset = -50
    const elementPosition = element.getBoundingClientRect().top + window.scrollY
    const offsetPosition = elementPosition + offset
    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth'
    })
  }
}
</script>

<template>
  <div>
    <div
      class="mx-auto flex w-full flex-col items-center gap-8 px-4 md:px-10 lg:flex-row lg:gap-12 lg:px-12 xl:px-20 2xl:max-w-[1440px] 2xl:px-0"
    >
      <!-- LEFT SECTION -->
      <div class="relative">
        <div class="">
          <img class="w-96 rounded-xl object-cover" src="../assets/img/buerogebäude.webp" alt="" />

          <img
            class="absolute -left-4 -top-4 w-10 animate-spin-slow md:-left-10 md:-top-12 md:w-24"
            src="../assets/img/vectors/circle.png"
            alt=""
          />

          <div class="mt-4 flex items-center justify-center gap-2.5">
            <span class="font-body text-6xl font-bold text-primary">NEU</span>
            <p class="font-title text-xl font-bold">JUNG · <br class="hidden" />AGIL</p>
          </div>
        </div>
      </div>

      <!-- RIGHT SECTION -->
      <div class="grid place-items-center text-center lg:w-2/3 lg:place-items-start lg:text-start">
        <h3 class="mb-5 flex items-end gap-3 text-xl font-medium text-subtitle">
          <img class="mb-1.5 w-7" src="../assets/img/broom-icon.svg" alt="Broom Icon" />ÜBER UNS
        </h3>

        <h2
          class="mb-6 text-[28px] font-bold leading-[36px] sm:text-4xl sm:leading-[46px] lg:text-[44px]"
        >
          Unser Versprechen ist es, stets
          <br class="hidden 2xl:block" />die
          <span class="font-title text-primary">besten Dienste </span> zu liefern.
        </h2>

        <p class="font-light leading-7 text-description xl:text-justify">
          Unser junges und engagiertes Team bei EL macht uns nicht nur zur einer Reinigungsfirma;
          Wir sind Ihr Partner in Sachen Sauberkeit und Professionalität. Unsere Mission ist es,
          Ihnen erstklassige Dienstleistungen zu bieten, die Ihre Wünsche zu allem Maße erfüllen.
        </p>

        <div class="mt-8 grid gap-2 gap-x-10 sm:grid-cols-2 md:gap-y-2.5 xl:gap-x-10">
          <div v-for="check in checks" :key="check.index" class="flex items-center">
            <ShieldCheck class="mr-2 h-8 w-8 fill-primary stroke-white" />
            <p class="font-medium tracking-wide">{{ check.description }}</p>
          </div>
        </div>

        <Button @click="scrollTo('contact-us')" class="mt-8 h-14 px-6"
          ><NotebookPen class="mr-1.5 w-5" />Angebot anfordern</Button
        >
      </div>
    </div>
  </div>
</template>
