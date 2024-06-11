<script setup lang="ts">
import Button from './ui/button/Button.vue'

import { Phone, PhoneCall } from 'lucide-vue-next'
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-20 2xl:px-0">
      <div class="grid gap-10">
        <div class="grid gap-5 text-white">
          <h3
            class="break-words text-center text-[26px] font-bold leading-7 tracking-wide md:text-start"
          >
            Ihr maßgeschneidertes Reinigungsangebot
          </h3>
          <p class="text-center font-light leading-7 tracking-wide opacity-90 md:text-start">
            Jeder Raum hat seine eigenen Anforderungen, wenn es um Sauberkeit geht. Bei EL-Reinigung
            verstehen wir das und entwickeln daher speziell auf Ihre Bedürfnisse zugeschnittene
            Reinigungslösungen. Kontaktieren Sie uns für ein individuelles Angebot und erfahren Sie,
            wie wir Ihre Räume nicht nur sauberer, sondern auch gesünder und einladender machen
            können.
          </p>
        </div>

        <div
          class="relative grid place-items-center rounded-lg bg-secondary px-3.5 py-12 md:px-10 lg:flex lg:gap-44"
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
              Sind Sie bereit, Ihre Räumlichkeiten zu transformieren? Rufen Sie uns an oder senden
              Sie uns eine E-Mail, um Ihre individuelle Reinigungslösung zu besprechen. Unser
              engagiertes Team ist bestrebt, Ihre Erwartungen zu übertreffen und eine Umgebung zu
              schaffen, die Reinheit und Komfort ausstrahlt.
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
