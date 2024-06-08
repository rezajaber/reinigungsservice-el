<script setup lang="ts">
import CardComponent from '@/components/ServiceCard.vue'

import {
  Carousel,
  CarouselContent,
  CarouselItem,
  CarouselNext,
  CarouselPrevious
} from '@/components/ui/carousel'
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-16 2xl:px-20">
      <!-- TITLE SECTION -->
      <div class="mb-24 lg:mb-14">
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

      <!-- CAROUSEL SECTION -->
      <Carousel
        class="h-full py-4"
        :opts="{
          align: 'start'
        }"
      >
        <CarouselContent>
          <CarouselItem v-for="(_, index) in 5" :key="index" class="md:basis-1/2 lg:basis-1/3">
            <CardComponent
              image="../src/assets/img/service-card-one.jpeg"
              title="Window Cleaning"
              description="General Cleaning is a House a cleaning this includes dusting, floors, wiping."
              link="/window-cleaning"
            />
          </CarouselItem>
        </CarouselContent>

        <CarouselPrevious class="lg:mr-16" />
        <CarouselNext />
      </Carousel>
    </div>
  </div>
</template>
