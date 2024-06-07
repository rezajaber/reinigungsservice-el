<script setup lang="ts">
import Header from '../components/Header.vue'
import Hero from '../components/Hero.vue'
import AboutUs from '../components/AboutUs.vue'

import Einsatzgebiete from '../components/Einsatzgebiete.vue'
import Card from '../components/Card.vue'

import ContactUs from '../components/ContactUs.vue'
import Footer from '../components/Footer.vue'

import { Phone, PhoneCall } from 'lucide-vue-next'
</script>

<template>
  <div>
    <Header class="fixed inset-x-0 top-0 z-10 bg-white" />
    <Hero class="my-20 lg:my-24" />
    <AboutUs class="" />
    <Einsatzgebiete class="mb-12 mt-28 px-5 md:px-20 xl:px-0" />
    <!-- Additional services section with highlighted information -->

    <ContactUs id="contact-us" class="bg-primary px-5 py-8 md:px-20 md:py-20 xl:px-0" />
    <Footer class="bg-popover-foreground py-12 lg:px-20" />
  </div>
</template>
