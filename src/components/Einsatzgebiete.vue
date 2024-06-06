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
  <div
    class="mx-auto flex max-w-[1080px] flex-col justify-center gap-10 lg:flex-row lg:items-center"
  >
    <img
      src="../assets/img/hamburg.jpg"
      alt="Hamburg"
      class="hidden h-96 w-full rounded-lg object-cover lg:block lg:h-[450px]"
    />

    <!-- ENGAGEMENT TEXT -->
    <div class="mx-auto mb-8 grid max-w-[1080px] gap-6 text-center md:text-start">
      <h3 class="break-words text-[26px] font-bold leading-7 tracking-wide text-primary">
        Unsere Einsatzgebiete in Hamburg
      </h3>
      <p class="font-light leading-7 tracking-wide">
        Wir sind stolz darauf, in ganz Hamburg für Sauberkeit und Ordnung zu sorgen. Von Altona bis
        Zollenspieker – unser Team ist in allen Stadtteilen der Hansestadt für Sie im Einsatz:
      </p>

      <img
        src="../assets/img/hamburg.jpg"
        alt="Hamburg"
        class="h-96 w-full rounded-lg object-cover md:h-[550px] lg:hidden"
      />

      <div class="flex flex-wrap justify-center gap-2 lg:justify-start">
        <Button size="sm" class="w-fit" v-for="(stadtteil, index) in stadtteile" :key="index">{{
          stadtteil
        }}</Button>
      </div>
    </div>
  </div>
</template>
