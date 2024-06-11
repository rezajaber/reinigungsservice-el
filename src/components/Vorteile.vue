<script setup lang="ts">
import {
  SearchCheck,
  ClipboardList,
  HeartHandshake,
  BriefcaseMedical,
  Building2,
  GraduationCap
} from 'lucide-vue-next'

const icons = [
  SearchCheck,
  ClipboardList,
  HeartHandshake,
  BriefcaseMedical,
  Building2,
  GraduationCap
]
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
  },
  {
    id: 4,
    icon: 'BriefcaseMedical',
    title: 'Praxen',
    description:
      'Wir bieten spezialisierte Reinigungsdienste für Praxen an, um eine hygienische und einladende Umgebung für Patienten und Personal zu gewährleisten.'
  },
  {
    id: 5,
    icon: 'Building2',
    title: 'Firmen',
    description:
      'Unsere professionellen Reinigungskräfte sorgen für saubere und produktive Arbeitsbereiche in Unternehmen jeder Größe.'
  },
  {
    id: 6,
    icon: 'GraduationCap',
    title: 'Sozialeinrichtungen',
    description:
      'Wir bieten umfassende Reinigungsdienste für Sozialeinrichtungen, um sicherzustellen, dass die Räumlichkeiten sicher und angenehm für alle Bewohner und Besucher sind.'
  }
]
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-20 2xl:px-0">
      <div class="mb-20">
        <h3
          class="mb-6 flex items-end justify-center gap-3 text-xl font-medium text-subtitle lg:justify-start"
        >
          <img class="mb-1.5 w-7" src="../assets/img/broom-icon.svg" alt="Broom Icon" />WIR BIETEN
          IHNEN
        </h3>

        <h1
          class="text-center text-[28px] font-bold leading-9 md:text-4xl md:leading-[46px] lg:text-start lg:text-[44px]"
        >
          Unsere
          <span class="font-title text-primary">Versprechen</span>
          <br class="hidden md:block" />
          für Ihre Zufriedenheit
        </h1>
      </div>

      <div class="grid gap-5 md:grid-cols-2 md:gap-8 lg:grid-cols-3 lg:gap-y-5">
        <div
          v-for="(vorteil, index) in vorteile"
          :key="vorteil.id"
          class="card group relative flex flex-col rounded-lg bg-white p-8 duration-500 ease-in-out hover:scale-[1.03]"
        >
          <component
            :is="icons[index]"
            class="icon mb-4 h-20 w-20 items-end rounded-full bg-[#F4F7FF] stroke-icon stroke-1 p-5 duration-300 ease-in-out group-hover:bg-icon group-hover:stroke-white md:h-[90px] md:w-[90px] lg:h-24 lg:w-24 lg:p-6"
          />
          <h3
            class="mb-[10px] mt-2 break-words text-start text-[26px] font-bold leading-[31px] tracking-wide text-icon"
          >
            {{ vorteil.title }}
          </h3>
          <p class="text-start text-sm leading-7 tracking-wide text-description lg:mt-3">
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

.card:hover .icon {
  animation: spinX 0.5s ease-in-out;
}

@keyframes spinX {
  from {
    transform: rotateY(0deg);
  }
  to {
    transform: rotateY(360deg);
  }
}
</style>
