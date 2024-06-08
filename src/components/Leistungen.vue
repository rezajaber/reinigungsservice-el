<script setup lang="ts">
import CardComponent from '../components/ServiceCard.vue'
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px]">
      <div class="">
        <span class="flex items-end gap-3 text-xl font-medium text-subtitle">
          <img class="mb-1.5 w-7" src="../assets/img/broom-icon.svg" alt="Broom Icon" />ABOUT
          COMPANY
        </span>

        <h1 class="mt-6 text-5xl font-bold">
          Our Promise Is To Deliver Only <br />The Best
          <span class="font-title text-primary">Services</span>
        </h1>
      </div>

      <CardComponent
        image="../src/assets/img/service-card-one.jpeg"
        title="Window Cleaning"
        description="General Cleaning is a House a cleaning this includes dusting, floors, wiping."
        link="/window-cleaning"
      />
    </div>
  </div>
</template>
