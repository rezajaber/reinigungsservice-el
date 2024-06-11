<script setup lang="ts">
import { Warehouse, ArrowUpRight } from 'lucide-vue-next'
import Button from './ui/button/Button.vue'
import { Card, CardContent } from '@/components/ui/card'
import {
  Carousel,
  CarouselContent,
  CarouselItem,
  CarouselNext,
  CarouselPrevious
} from '@/components/ui/carousel'

import serviceOne from '../assets/img/service/grundreinigung.webp'
import serviceTwo from '../assets/img/service/desinfektion.webp'
import serviceThree from '../assets/img/service/buero.webp'
import serviceFour from '../assets/img/service/lagerreinigung.webp'
import serviceFive from '../assets/img/service/treppenhaus.webp'
import serviceSix from '../assets/img/service/praxisreinigung.webp'
import serviceSeven from '../assets/img/service/sozialeinrichtung.webp'
import serviceEight from '../assets/img/service/unterhaltsreinigung.webp'
import serviceNine from '../assets/img/service/glasundfenster.webp'

const services = [
  {
    src: serviceOne,
    alt: 'Grundreinigung',
    title: 'Grundreinigung',
    description:
      'Unsere Grundreinigung bietet eine umfassende und gründliche Reinigungslösung für Ihr Zuhause oder Büro, besonders nützlich bei Umzügen oder saisonalen Tiefenreinigungen. Dazu gehören auch Möbelmontage und Raumrenovierung, um Ihren Raum von Grund auf zu erneuern und eine frische, saubere Umgebung zu schaffen.'
  },
  {
    src: serviceTwo,
    alt: 'Desinfektion',
    title: 'Desinfektion',
    description:
      'Wir bieten fachgerechte Desinfektionsdienste, die ideal für die Entrümpelung von Kellern und die Auflösung von Unternehmen sind. Unsere Methoden sind sowohl effizient als auch umweltfreundlich, um sicherzustellen, dass alle betroffenen Bereiche sicher und frei von schädlichen Keimen und Bakterien sind.'
  },
  {
    src: serviceThree,
    alt: 'Büroreinigung',
    title: 'Büroreinigung',
    description:
      'Unsere professionelle Büroreinigung passt sich Ihren individuellen Bedürfnissen an, von einfachen Auffrischungen bis hin zu komplexen Renovierungen. Wir sorgen dafür, dass Ihr Arbeitsplatz stets sauber, organisiert und produktivitätsfördernd ist, damit Sie und Ihr Team in einer angenehmen Umgebung arbeiten können.'
  },
  {
    src: serviceFour,
    alt: 'Lagerreinigung',
    title: 'Lagerreinigung',
    description:
      'Unsere spezialisierten Reinigungsdienste für Lager und Industrieanlagen gewährleisten eine saubere und effiziente Arbeitsumgebung. Wir entfernen hartnäckigen Schmutz, Staub und Ablagerungen, um die Betriebssicherheit zu erhöhen und die Lebensdauer Ihrer Anlagen zu verlängern.'
  },
  {
    src: serviceFive,
    alt: 'Treppenhausreinigung',
    title: 'Treppenhausreinigung',
    description:
      'Mit unserer regelmäßigen und gründlichen Treppenhausreinigung sorgen wir für Sicherheit und Sauberkeit in Wohngebäuden und Bürokomplexen. Wir entfernen Schmutz und Abfälle, polieren Geländer und sorgen für ein einladendes Erscheinungsbild, das Bewohner und Besucher gleichermaßen schätzen werden.'
  },
  {
    src: serviceSix,
    alt: 'Sozialeinrichtungen',
    title: 'Sozialeinrichtungen',
    description:
      'Unsere Reinigung für Sozialeinrichtungen ist gründlich und empathisch, um ein sicheres und hygienisches Umfeld für Betreuer und Betreute zu schaffen. Wir berücksichtigen die speziellen Anforderungen und sensiblen Bedürfnisse dieser Umgebungen und bieten flexible Zeitpläne an, um den täglichen Betrieb nicht zu stören. So gewährleisten wir stets eine einwandfreie Sauberkeit und Sicherheit.'
  },
  {
    src: serviceSeven,
    alt: 'Praxisreinigung',
    title: 'Praxisreinigung',
    description:
      'Unsere Praxisreinigung richtet sich nach spezifischen Reinigungsprotokollen für medizinische und zahnmedizinische Praxen, die höchste Hygienestandards erfordern. Wir entfernen gründlich alle Verunreinigungen, um eine sterile Umgebung zu gewährleisten, die sowohl für Patienten als auch für das medizinische Personal sicher ist.'
  },
  {
    src: serviceEight,
    alt: 'Unterhaltsreinigung',
    title: 'Unterhaltsreinigung',
    description:
      'Unsere regelmäßige Unterhaltsreinigung für Büros und Geschäftsräume schafft kontinuierlich saubere und professionelle Umgebungen. Wir bieten flexible Zeitpläne und maßgeschneiderte Reinigungspläne an, um sicherzustellen, dass Ihre Räumlichkeiten stets repräsentativ und betriebsbereit sind.'
  },
  {
    src: serviceNine,
    alt: 'Glas und Fensterreinigung',
    title: 'Glas-/Fensterreinigung',
    description:
      'Unsere fachmännische Reinigung von Glasflächen und Fenstern sorgt für eine klare Sicht und blendende Sauberkeit in allen Gebäuden. Ob hochgelegene Fenster oder empfindliche Glasstrukturen – wir verwenden spezielle Techniken und Ausrüstungen, um strahlende Ergebnisse ohne Streifen oder Rückstände zu erzielen.'
  }
]
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1440px] px-4 md:px-10 lg:px-12 xl:px-20 2xl:px-0">
      <!-- TITLE SECTION -->
      <div class="relative mb-24 lg:mb-14">
        <h3
          class="mb-6 flex items-end justify-center gap-3 text-xl font-medium text-subtitle lg:justify-start"
        >
          <img
            class="mb-1.5 w-7"
            src="../assets/img/broom-icon.svg"
            alt="Broom Icon"
          />PROFESSIONELLER SERVICE
        </h3>

        <h1
          class="text-center text-[28px] font-bold leading-9 md:text-4xl md:leading-[46px] lg:text-start lg:text-[44px]"
        >
          Unsere
          <span class="font-title text-primary">Reinigungsdienste</span>
          <br class="hidden md:block" />
          direkt vor Ihrer Tür
        </h1>

        <img
          class="absolute -right-2 -top-5 animate-bounce-slow"
          src="../assets/img/vectors/blue-stars.png"
          alt=""
        />
      </div>

      <!-- CAROUSEL SECTION -->
      <Carousel
        class="relative w-full outline-none"
        :opts="{
          align: 'start'
        }"
      >
        <CarouselContent>
          <CarouselItem
            v-for="(service, index) in services"
            :key="index"
            class="sm:basis-1/2 lg:basis-1/3"
          >
            <div class="p-1">
              <Card>
                <CardContent class="flex aspect-square items-center justify-center p-0">
                  <div class="">
                    <img :src="service.src" class="h-56 w-full object-cover" alt="Card image" />

                    <div
                      class="relative flex flex-grow flex-col items-center justify-between px-6 py-4 text-center"
                    >
                      <div class="rhombus absolute -top-11 flex w-56 justify-center bg-white py-6">
                        <Warehouse class="h-10 w-10 stroke-primary stroke-1" />
                      </div>

                      <h3 class="mt-8 text-2xl font-bold">{{ service.title }}</h3>
                      <p
                        class="no-scrollbar mt-3.5 h-40 overflow-y-scroll text-sm font-light leading-7 text-description"
                      >
                        {{ service.description }}
                      </p>
                      <Button class="my-6 h-11 px-8"
                        >Mehr Info<ArrowUpRight class="ml-1.5 h-5 w-5"
                      /></Button>
                    </div>
                  </div>
                </CardContent>
              </Card>
            </div>
          </CarouselItem>
        </CarouselContent>
        <CarouselPrevious class="lg:mr-16" />
        <CarouselNext />
      </Carousel>
    </div>
  </div>
</template>

<style scoped>
.rhombus {
  clip-path: polygon(50% 0, 100% 50%, 50% 100%, 0% 50%);
}

.broom {
  animation: moveLeftRight 2s infinite; /* Adjust duration as needed */
}

@keyframes moveLeftRight {
  0% {
    transform: translateX(0);
  }
  50% {
    transform: translateX(-20px); /* Move left by 20 pixels */
  }
  100% {
    transform: translateX(0);
  }
}
</style>
