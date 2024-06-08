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
    <AboutUs class="py-20" />

    <div class="bg-[#EBF3FE]">
      <Vorteile class="py-20" />
      <Einsatzorte class="py-20" />
    </div>

    <Leistungen class="py-20" />

    <Einsatzgebiete class="mb-12 mt-28 px-5 md:px-20 xl:px-0" />
    <!-- Additional services section with highlighted information -->

    <ContactUs id="contact-us" class="bg-primary px-5 py-8 md:px-20 md:py-20 xl:px-0" />
    <Footer class="bg-popover-foreground py-12 lg:px-20" />
  </div>
</template>
