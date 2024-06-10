<script setup lang="ts">
import { RouterView } from 'vue-router'
import { onMounted, ref } from 'vue'

const showPreloader = ref(true)

onMounted(() => {
  setTimeout(() => {
    showPreloader.value = false
  }, 1500)
})
</script>

<template>
  <Transition name="fade">
    <div
      v-if="showPreloader"
      class="dark fixed inset-0 z-50 flex items-center justify-center bg-background text-xl tracking-wide text-white"
    >
      <img src="/src/assets/img/logo.png" class="h-24 w-24 animate-bounce" alt="" />
    </div>
  </Transition>

  <Transition name="fade">
    <RouterView />
  </Transition>
</template>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 1500ms ease; /* Transition adjusted to 2.5 seconds */
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
