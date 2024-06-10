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
      'Von der Umzugsplanung über den Möbel- und Kistentransport bis hin zu optionalen Services wie dem Auspacken der Umzugskartons, der Möbelmontage sowie Reinigungs-, Maler- und Renovierungsarbeiten. Wir bieten Ihnen ein umfangreiches, individuell angepasstes Angebot und unterstützen Sie mit unseren Services für Ihren Umzug. Wir verhelfen Ihnen zu einem erfolgreichen, angenehmen und besonders für Sie stressfreien Umzug.'
  },
  {
    src: serviceTwo,
    alt: 'Desinfektion',
    title: 'Desinfektion',
    description:
      'Unser Team steht Ihnen zur Verfügung, wenn Sie ein Unternehmen auflösen, eine Erbschaft erhalten oder Ihren Keller oder Ihre Garage aufräumen müssen. Wir übernehmen die Haushaltsauflösung, schaffen Platz, verwerten nützliche Gegenstände und entsorgen Abfälle jeglicher Art (privat/gewerblich) unter Berücksichtigung der Umweltstandards.'
  },
  {
    src: serviceThree,
    alt: 'Büroreinigung',
    title: 'Büroreinigung',
    description:
      'Wir bieten Abriss- oder Abbrucharbeiten für Teile eines Gebäudes/Anbaus im Innen- oder Außenbereich, komplette Innenraum-Neugestaltung, Erstellung einer Öffnung in der Wand, Einsetzen/Entfernen eines Kamins oder Terrassenabbruch in Ihrem Garten. Mit unserer Expertise in diesem Bereich können wir jede Arbeit flexibel, schnell und problemlos für Sie und nach Ihren speziellen Wünschen erledigen.'
  },
  {
    src: serviceFour,
    alt: 'Hausmeisterservice',
    title: 'Grundreinigung',
    description:
      'Sie suchen einen flexiblen und engagierten Hausmeister Ihres Vertrauens für Ihre Immobilie oder Ihr Unternehmen? Oder Sie brauchen nur für einen kleinen Auftrag oder für eine bestimmte kurze Zeit die Dienste eines Hausmeisters? Bei WWEHGER stehen wir mit unseren spezialisierten Hausmeisterdiensten zur Verfügung und freuen uns auf Ihre Anfrage!'
  },
  {
    src: serviceFive,
    alt: 'Lagerreinigung',
    title: 'Lagerreinigung',
    description:
      'Sie haben ein kleines Projekt im Garten vor und benötigen jemanden, der Ihre Vision versteht und umsetzen kann, oder wollen zuverlässige Helfer für Rasenmähen, Hecke schneiden, Unkraut zupfen und Co.? Sie besitzen oder managen eine Immobilie oder ein Unternehmen und auch dort soll es in Ihrem Vorgarten gepflegt und ordentlich aussehen? Unser Team ist für Sie und Ihre Wünsche da! Vereinbaren Sie ein Beratungsgespräch oder erfragen Sie ein unverbindliches Angebot.'
  },
  {
    src: serviceSix,
    alt: 'Treppenhausreinigung',
    title: 'Treppenhausreinigung',
    description:
      'Der zuverlässige Winterdienst für Sie als Privatperson im Vorgarten, für Ihr Büro/Gebäude, ganze Straßen oder sogar mehrere Bezirke und Routen - und das, wenn gewünscht, jederzeit im 24/7-Notfall-Winterdienst!'
  },
  {
    src: serviceSeven,
    alt: 'Praxisreinigung',
    title: 'Praxisreinigung',
    description:
      'Gebäudereinigung für Einzel- oder Großraumbüros, Bürokomplexe, Industriegebäude oder einfache Mehrfamilienhäuser - wir von WWEHGER stehen mit unserem professionellen Team für hygienische Sauberkeit bereit und krempeln die Ärmel hoch.'
  },
  {
    src: serviceEight,
    alt: 'Unterhaltsreinigung',
    title: 'Unterhaltsreinigung',
    description:
      'Gebäudereinigung für Einzel- oder Großraumbüros, Bürokomplexe, Industriegebäude oder einfache Mehrfamilienhäuser - wir von WWEHGER stehen mit unserem professionellen Team für hygienische Sauberkeit bereit und krempeln die Ärmel hoch.'
  },
  {
    src: serviceNine,
    alt: 'Glas und Fensterreinigung',
    title: 'Glas und Fensterreinigung',
    description:
      'Gebäudereinigung für Einzel- oder Großraumbüros, Bürokomplexe, Industriegebäude oder einfache Mehrfamilienhäuser - wir von WWEHGER stehen mit unserem professionellen Team für hygienische Sauberkeit bereit und krempeln die Ärmel hoch.'
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
          Trusted Cleaning <span class="font-title text-primary">Services</span>
          <br class="hidden md:block" />
          On Your Door
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
                        class="no-scrollbar mt-3.5 h-48 overflow-y-scroll text-sm font-light leading-7 text-description"
                      >
                        {{ service.description }}
                      </p>
                      <Button class="my-6 h-11 px-8"
                        >See More<ArrowUpRight class="ml-1.5 h-5 w-5"
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
