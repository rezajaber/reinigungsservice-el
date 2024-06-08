<script setup lang="ts">
import Button from './ui/button/Button.vue'

import { Phone, PhoneCall } from 'lucide-vue-next'
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-16 2xl:px-20">
      <div class="grid gap-10">
        <div class="grid gap-5 text-white">
          <h3
            class="break-words text-center text-[26px] font-bold leading-7 tracking-wide md:text-start"
          >
            Ihr individuelles Reinigungsangebot anfordern
          </h3>
          <p class="text-center font-light leading-7 tracking-wide opacity-90 md:text-start">
            Wir verstehen, dass jedes Gebäude und jede Reinigungsaufgabe ihre eigenen einzigartigen
            Anforderungen hat. Deshalb bieten wir maßgeschneiderte Reinigungslösungen, die speziell
            auf Ihre individuellen Bedürfnisse zugeschnitten sind. Fordern Sie jetzt Ihr
            persönliches Angebot an und lassen Sie uns gemeinsam herausfinden, wie wir Ihr Umfeld
            nicht nur sauberer, sondern auch gesünder und angenehmer gestalten können.
          </p>
        </div>

        <div
          class="grid place-items-center rounded-lg bg-secondary px-3.5 py-12 md:px-10 lg:flex lg:gap-44"
        >
          <div class="grid place-items-center gap-4 text-center lg:place-items-start">
            <div class="grid place-items-center lg:flex lg:items-center lg:gap-4">
              <PhoneCall class="fill-primary stroke-primary" />
              <h3 class="text-2xl font-bold tracking-wide text-primary">
                Kontaktieren Sie uns jetzt
              </h3>
            </div>
            <p
              class="mb-10 text-center font-light leading-7 tracking-wide text-primary lg:mb-0 lg:text-start"
            >
              Sind Sie bereit für eine tadellose Geschäftsumgebung? Rufen Sie uns an oder senden Sie
              uns eine E-Mail, um Ihre maßgeschneiderte Reinigungslösung zu planen. Unser
              professionelles Team freut sich darauf, Ihre Räumlichkeiten in neuem Glanz erstrahlen
              zu lassen und eine saubere, einladende Atmosphäre zu schaffen.
            </p>
          </div>

          <div class="grid gap-2 sm:flex lg:grid">
            <a href="tel:+49 174 9524843">
              <Button type="button" class="w-full"> +49 174 9524843 </Button>
            </a>
            <a href="mailto:info@el-reinigung.de">
              <Button class="bg-primary text-white">info@el-reinigung.de</Button>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
