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
    <Hero class="" />
    <AboutUs class="" />

    <div class="bg-[#EBF3FE]">
      <Vorteile class="" />
      <Einsatzorte class="" />
    </div>

    <Leistungen class="" />

    <Einsatzgebiete class="" />
    <!-- Additional services section with highlighted information -->

    <ContactUs id="contact-us" class="x bg-primary" />
    <Footer class="bg-popover-foreground" />
  </div>
</template>
