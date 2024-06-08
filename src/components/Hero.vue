<script setup lang="ts">
import Button from './ui/button/Button.vue'
import { ClipboardList, NotebookPen } from 'lucide-vue-next'
</script>

<template>
  <div>
    <div class="relative">
      <img
        class="h-[700px] w-full transform object-cover transition-transform duration-500 ease-in-out hover:scale-105 lg:h-[800px]"
        src="../assets/img/hero.jpeg"
        alt="Hero Image"
      />

      <!-- Gradient overlay -->
      <img
        class="absolute top-0 h-full w-full object-cover"
        src="../assets/img/hero-overlay.png"
        alt="Hero Overlay"
      />

      <div class="absolute inset-0 mx-auto flex items-center text-white 2xl:max-w-[1440px]">
        <div class="grid place-items-center lg:place-items-start">
          <span class="flex items-end gap-3 text-xl font-medium text-subtitle">
            <img class="mb-1.5 w-7" src="../assets/img/broom-icon.svg" alt="Broom Icon" />CLEAN YOUR
            HOME
          </span>

          <h1
            class="mt-8 text-center text-4xl font-bold tracking-wide text-white sm:text-5xl md:text-6xl md:leading-[65px] lg:text-start"
          >
            RESIDENTIAL REVIVE <br />CLEAN
            <span class="outlined font-title text-transparent">SERVICE</span>
          </h1>

          <p
            class="mt-5 text-center text-base font-light leading-7 tracking-wide text-white lg:text-start"
          >
            With our professional cleaning service, you can count on us to provide a meticulous and
            top-tier <br class="hidden lg:block" />
            cleaning experience for both residential and commercial spaces, Kitchen, carpet, toilet,
            leaving <br class="hidden lg:block" />your environment spotless and revitalized on every
            occasion.
          </p>

          <div class="mt-8 grid gap-4 sm:flex">
            <Button class="h-14 px-6"><NotebookPen class="mr-1.5 w-5" />Angebot anfordern</Button>
            <Button class="h-14 px-6"><ClipboardList class="mr-2 w-5" />Unsere Leistungen</Button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.outlined {
  color: transparent;
  -webkit-text-stroke: 2px hsl(var(--primary)); /* adjust stroke width and color */
}
</style>
