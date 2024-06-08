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
    <Header class="fixed inset-x-0 top-0 z-10 bg-white" />
    <Hero class="py-20 lg:py-24" />
    <AboutUs class="pb-20 lg:pb-24" />

    <div class="grid gap-20 bg-[#EBF3FE] py-20 lg:py-24">
      <Vorteile class="" />
      <Einsatzorte class="" />
    </div>

    <Leistungen class="py-20 lg:py-24" />

    <Einsatzgebiete class="pb-20 lg:pb-24" />
    <!-- Additional services section with highlighted information -->

    <ContactUs id="contact-us" class="bg-primary py-20 lg:py-24" />
    <Footer class="bg-popover-foreground py-8 lg:py-12" />
  </div>
</template>
