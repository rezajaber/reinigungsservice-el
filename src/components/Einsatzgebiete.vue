<script setup lang="ts">
import Button from './ui/button/Button.vue'

const stadtteile = [
  'Altona',
  'Sternschanze',
  'Barmbek',
  'Blankenese',
  'Billstedt',
  'Finkenwerder',
  'HafenCity',
  'Horn',
  'Wandsbek',
  'Jungfernstieg',
  'Hauptbahnhof',
  'Hammerbrook',
  'Veddel',
  'Wilhelmsburg',
  'Harburg',
  'Harburg Rathaus',
  'Heimfeld',
  'Neuwiedenthal',
  'Neugraben',
  'Neu Wulmstorf',
  'Fischbek',
  'Meckelfeld',
  'Marmstorf',
  'Sinstorf',
  'Wilstorf',
  '...'
]
</script>

<template>
  <div class="">
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-20 2xl:px-0">
      <div class="flex flex-col justify-center gap-20 lg:flex-row lg:items-center">
        <!-- LEFT SECTION -->
        <div
          class="grid place-items-center text-center lg:w-1/2 lg:place-items-start lg:text-start"
        >
          <h3 class="mb-5 flex items-end gap-3 text-xl font-medium text-subtitle">
            <img class="mb-1.5 w-7" src="../assets/img/broom-icon.svg" alt="Broom Icon" />ABOUT
            COMPANY
          </h3>

          <h2
            class="mb-6 text-[28px] font-bold leading-[36px] sm:text-4xl sm:leading-[46px] lg:text-[44px]"
          >
            Unsere <span class="font-title text-primary">Einsatzgebiete</span> in Hamburg
          </h2>

          <p class="mb-8 font-light leading-7 text-description xl:text-justify">
            Wir sind stolz darauf, in ganz Hamburg für Sauberkeit und Ordnung zu sorgen. Von Altona
            bis Zollenspieker – unser Team ist in allen Stadtteilen der Hansestadt für Sie im
            Einsatz:
          </p>

          <!-- UP SECTION -->
          <img
            class="mb-8 h-96 rounded-lg object-cover lg:hidden"
            src="../assets/img/hamburg.webp"
            alt=""
          />

          <div class="flex flex-wrap justify-center gap-2 lg:justify-start">
            <Button size="sm" class="w-fit" v-for="(stadtteil, index) in stadtteile" :key="index">{{
              stadtteil
            }}</Button>
          </div>
        </div>

        <!-- RIGHT SECTION -->
        <div class="lg:w-1/2">
          <img
            class="hidden rounded-lg object-cover lg:block"
            src="../assets/img/hamburg.webp"
            alt=""
          />
        </div>
      </div>
    </div>
  </div>
</template>
