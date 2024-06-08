<script setup lang="ts">
import { SearchCheck, ClipboardList, HeartHandshake } from 'lucide-vue-next'

import Button from './ui/button/Button.vue'

const vorteile = [
  {
    id: 1,
    icon: 'SearchCheck',
    title: 'Outdoor Service',
    description:
      'Lorem ipsum dolor sit amet consectetur. Ut tellus suspendisse nulla aliquam. Risus pretium nisi amet facilisis.'
  },
  {
    id: 2,
    icon: 'ClipboardList',
    title: 'House Cleaning',
    description:
      'Lorem ipsum dolor sit amet consectetur. Ut tellus suspendisse nulla aliquam. Risus pretium nisi amet facilisis.'
  },
  {
    id: 3,
    icon: 'HeartHandshake',
    title: 'Office Cleaning',
    description:
      'Lorem ipsum dolor sit amet consectetur. Ut tellus suspendisse nulla aliquam. Risus pretium nisi amet facilisis.'
  }
]

const icons = [SearchCheck, ClipboardList, HeartHandshake]
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px]">
      <div class="flex flex-wrap gap-x-10 gap-y-[72px]">
        <div
          v-for="(vorteil, index) in vorteile"
          :key="vorteil.id"
          class="group relative flex w-[420px] flex-col rounded-xl bg-white px-8 pb-10 pt-16 shadow-lg sm:w-[330px] md:w-[340px] lg:w-[472px] xl:w-[440px]"
        >
          <component
            :is="icons[index]"
            class="stroke-icon group-hover:bg-icon absolute -top-12 h-20 w-20 rounded-full bg-[#F4F7FF] stroke-1 p-5 duration-300 ease-in-out group-hover:stroke-white md:h-[90px] md:w-[90px] lg:h-24 lg:w-24 lg:p-6"
          />
          <h3 class="text-icon mt-2 text-start text-2xl font-bold leading-7 tracking-wide">
            {{ vorteil.title }}
          </h3>
          <p class="text-description mt-3 text-start text-sm leading-7 tracking-wide lg:mt-3">
            {{ vorteil.description }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
