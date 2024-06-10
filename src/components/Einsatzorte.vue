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
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-20 2xl:px-0">
      <div class="grid gap-5 md:grid-cols-2 md:gap-8 lg:grid-cols-3">
        <div
          v-for="(vorteil, index) in vorteile"
          :key="vorteil.id"
          class="card group relative flex flex-col rounded-lg bg-white p-10 px-8 duration-500 ease-in-out hover:scale-[1.03]"
        >
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
