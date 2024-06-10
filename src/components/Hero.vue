<script setup lang="ts">
import Button from './ui/button/Button.vue'
import { ClipboardList, NotebookPen } from 'lucide-vue-next'

import { ref, onMounted } from 'vue'

const stars = ref<Array<{ top: string; left: string; delay: string }>>([])
const bubbles = ref<Array<{ size: string; left: string; delay: string }>>([])

const generateRandomPosition = () => {
  return {
    top: `${Math.random() * 100}%`,
    left: `${Math.random() * 50}%`
  }
}

const generateRandomDelay = () => {
  return `${Math.random() * 5}s`
}

const generateRandomSize = () => {
  return `${Math.random() * 3 + 1}rem` // Random size between 1rem and 4rem
}

const generateBubbleProperties = () => {
  return {
    size: generateRandomSize(),
    left: `${Math.random() * 50}%`, // Constrain to the left one-third of the screen
    delay: generateRandomDelay()
  }
}

onMounted(() => {
  for (let i = 0; i < 4; i++) {
    stars.value.push({
      ...generateRandomPosition(),
      delay: generateRandomDelay()
    })
  }

  for (let i = 0; i < 10; i++) {
    bubbles.value.push(generateBubbleProperties())
  }
})

const scrollTo = (id: string) => {
  const element = document.getElementById(id)
  if (element) {
    const offset = -50
    const elementPosition = element.getBoundingClientRect().top + window.scrollY
    const offsetPosition = elementPosition + offset
    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth'
    })
  }
}
</script>

<template>
  <div>
    <div class="relative">
      <img
        class="h-[700px] w-full transform object-cover transition-transform duration-500 ease-in-out hover:scale-105 lg:h-[800px]"
        src="../assets/img/hero.jpg"
        alt="Hero Image"
      />

      <!-- Gradient overlay -->
      <div class="">
        <img
          class="absolute top-0 h-full w-full object-cover"
          src="../assets/img/hero-overlay.png"
          alt="Hero Overlay"
        />

        <div class="hidden xl:block">
          <img
            class="star absolute top-0 animate-pulse object-cover opacity-50"
            src="../assets/img/vectors/star.svg"
            alt=""
            v-for="(star, index) in stars"
            :key="index"
            :style="{ top: star.top, left: star.left, animationDelay: star.delay }"
          />

          <div class="bubble-container">
            <img
              v-for="(bubble, index) in bubbles"
              :key="index"
              src="../assets/img/vectors/bubble.png"
              alt=""
              class="bubble absolute"
              :style="{
                width: bubble.size,
                height: bubble.size,
                left: bubble.left,
                animationDelay: bubble.delay
              }"
            />
          </div>
        </div>
      </div>

      <div
        class="absolute inset-0 mx-auto flex items-center px-4 text-white md:px-10 lg:px-12 xl:px-16 2xl:max-w-[1440px] 2xl:px-20"
      >
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
            <Button @click="scrollTo('contact-us')" class="h-14 px-6"
              ><NotebookPen class="mr-1.5 w-5" />Angebot anfordern</Button
            >
            <Button @click="scrollTo('service')" class="h-14 px-6"
              ><ClipboardList class="mr-2 w-5" />Unsere Leistungen</Button
            >
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

@keyframes pulse {
  0%,
  100% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.5);
  }
}

@keyframes float {
  0% {
    transform: translateY(1vh); /* Start from below the screen */
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    transform: translateY(-100vh); /* Adjust as necessary */
    opacity: 0;
  }
}

.bubble {
  animation: float 10s infinite;
}

.bubble-container {
  position: relative;
  width: 50%; /* Constrain to the left one-third of the screen */
  height: 100%;
}
</style>
