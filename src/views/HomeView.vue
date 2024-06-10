<script setup lang="ts">
import Header from '../components/Header.vue'
import Hero from '../components/Hero.vue'
import AboutUs from '../components/AboutUs.vue'
import Vorteile from '../components/Vorteile.vue'
import Einsatzorte from '../components/Einsatzorte.vue'
import Leistungen from '../components/Leistungen.vue'

import Einsatzgebiete from '../components/Einsatzgebiete.vue'

import ContactUs from '../components/ContactUs.vue'
import Footer from '../components/Footer.vue'
</script>

<template>
  <div>
    <Header class="fixed inset-x-0 top-0 z-50 bg-white" />
    <Hero class="py-20 lg:py-24" />

    <div class="relative">
      <AboutUs class="pb-20 lg:pb-24" />
      <img
        class="broom absolute -bottom-8 right-8 z-10"
        src="../assets/img/vectors/big-broom.png"
        alt=""
      />
    </div>

    <div class="grid gap-5 bg-[#EBF3FE] py-20 lg:py-24">
      <Vorteile class="" />
    </div>

    <div class="relative py-20 lg:py-24">
      <Leistungen id="service" />
      <img
        class="broom absolute -bottom-10 left-0 w-20 md:w-24"
        src="../assets/img/vectors/small-brush.png"
        alt=""
      />
    </div>

    <Einsatzgebiete class="bg-[#EBF3FE] py-20 lg:pb-24" />

    <div class="relative">
      <ContactUs id="contact-us" class="bg-primary/90 py-20 lg:py-24" />
      <div class="absolute -top-24 right-10 w-32 rotate-90 sm:-top-32 sm:w-48">
        <img class="broom" src="../assets/img/vectors/big-brush.png" alt="" />
      </div>
    </div>

    <Footer class="bg-popover-foreground py-8 lg:py-12" />
  </div>
</template>

<style scoped>
.broom {
  animation: moveLeftRight 2s infinite; /* Adjust duration as needed */
}
.trash-pack {
  animation: moveUpDown 2s infinite;
}

@keyframes moveLeftRight {
  0% {
    transform: translateX(0);
  }
  50% {
    transform: translateX(-20px); /* Move left by 10 pixels */
  }
  100% {
    transform: translateX(0);
  }
}
</style>
