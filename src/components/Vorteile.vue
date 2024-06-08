<script setup lang="ts">
import { SearchCheck, ClipboardList, HeartHandshake } from 'lucide-vue-next'
import Button from './ui/button/Button.vue'

const icons = [SearchCheck, ClipboardList, HeartHandshake]
const vorteile = [
  {
    id: 1,
    icon: 'SearchCheck',
    title: 'Unsere Präzision',
    description:
      'Unsere Arbeit zeichnet sich durch höchste Präzision aus, um sicherzustellen, dass jede Aufgabe mit äußerster Genauigkeit und Sorgfalt ausgeführt wird.'
  },
  {
    id: 2,
    icon: 'ClipboardList',
    title: 'Unsere Flexibilität',
    description:
      'Dank unserer Vielfalt an Services und unserer Flexibilität können wir uns leicht an die spezifischen Anforderungen unserer Kunden anpassen und maßgeschneiderte Lösungen liefern.'
  },
  {
    id: 3,
    icon: 'HeartHandshake',
    title: 'Unser Kundenservice',
    description:
      'Wir legen großen Wert auf exzellenten Kundenservice, um sicherzustellen, dass unsere Kunden jederzeit zufrieden sind. Unser engagiertes Team steht Ihnen zur Seite, um Ihre Anliegen zu hören und Ihnen zu helfen.'
  }
]
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-16 2xl:px-20">
      <div class="mb-24">
        <h3
          class="mb-6 flex items-end justify-center gap-3 text-xl font-medium text-subtitle lg:justify-start"
        >
          <img
            class="mb-1.5 w-7"
            src="../assets/img/broom-icon.svg"
            alt="Broom Icon"
          />PROFESSIONELLER SERVICE
        </h3>

        <h1
          class="text-center text-[28px] font-bold leading-9 md:text-4xl md:leading-[46px] lg:text-start lg:text-[44px]"
        >
          Trusted Cleaning <span class="font-title text-primary">Services</span>
          <br class="hidden md:block" />
          On Your Door
        </h1>
      </div>

      <div class="grid gap-20 md:grid-cols-2 md:gap-8 md:gap-y-20 lg:grid-cols-3">
        <div
          v-for="(vorteil, index) in vorteile"
          :key="vorteil.id"
          class="card group relative flex flex-col rounded-lg bg-white px-8 pb-10 pt-16 duration-500 ease-in-out hover:-translate-y-2 hover:scale-105"
        >
          <component
            :is="icons[index]"
            class="stroke-icon group-hover:bg-icon absolute -top-14 h-20 w-20 rounded-full bg-[#F4F7FF] stroke-1 p-5 duration-300 ease-in-out group-hover:stroke-white md:h-[90px] md:w-[90px] lg:h-24 lg:w-24 lg:p-6"
          />
          <h3
            class="text-icon mb-[10px] mt-2 text-start text-[26px] font-bold leading-[31px] tracking-wide"
          >
            {{ vorteil.title }}
          </h3>
          <p class="text-description text-start text-sm leading-7 tracking-wide lg:mt-3">
            {{ vorteil.description }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
}
</style>
