<script setup lang="ts">
import ServiceCard from '@/components/ServiceCard.vue'
import { Warehouse, ArrowUpRight } from 'lucide-vue-next'

import Button from './ui/button/Button.vue'
import { Card, CardContent } from '@/components/ui/card'
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
        class="relative w-full"
        :opts="{
          align: 'start'
        }"
      >
        <CarouselContent>
          <CarouselItem v-for="(_, index) in 5" :key="index" class="md:basis-1/2 lg:basis-1/3">
            <div class="p-1">
              <Card>
                <CardContent class="flex aspect-square items-center justify-center p-0">
                  <ServiceCard />
                </CardContent>
              </Card>
            </div>
          </CarouselItem>
        </CarouselContent>
        <CarouselPrevious class="lg:mr-16" />
        <CarouselNext />
      </Carousel>
    </div>
  </div>
</template>

<style scoped>
.rhombus {
  clip-path: polygon(50% 0, 100% 50%, 50% 100%, 0% 50%);
}
</style>
