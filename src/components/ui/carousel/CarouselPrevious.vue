<script setup lang="ts">
import { ArrowLeft } from 'lucide-vue-next'
import { useCarousel } from './useCarousel'
import type { WithClassAsProps } from './interface'
import { cn } from '@/lib/utils'
import { Button } from '@/components/ui/button'

const props = defineProps<WithClassAsProps>()

const { orientation, canScrollPrev, scrollPrev } = useCarousel()
</script>

<template>
  <div class="mr-16 flex justify-center">
    <Button
      :disabled="!canScrollPrev"
      :class="
        cn(
          'absolute h-12 w-14 touch-manipulation rounded-lg p-0',
          orientation === 'horizontal'
            ? '-top-14 -translate-y-1/2 lg:-top-20 lg:right-0'
            : '-top-12 left-1/2 -translate-x-1/2 rotate-90',
          props.class
        )
      "
      @click="scrollPrev"
    >
      <slot>
        <ArrowLeft class="h-4 w-4 text-current" />
      </slot>
    </Button>
  </div>
</template>
