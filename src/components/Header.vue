<script setup lang="ts">
import { Menu, Mail, Phone, PhoneCall, Smartphone } from 'lucide-vue-next'
import { Button } from '@/components/ui/button'
import {
  Dialog,
  DialogContent,
  DialogDescription,
  DialogHeader,
  DialogTitle,
  DialogTrigger
} from '@/components/ui/dialog'
import { Tooltip, TooltipContent, TooltipProvider, TooltipTrigger } from '@/components/ui/tooltip'

const scrollTo = (id: string, behavior: ScrollBehavior = 'auto') => {
  const element = document.getElementById(id)
  if (element) {
    element.scrollIntoView({ behavior })
  }
}
</script>

<template>
  <div class="shadow-md">
    <div
      class="mx-auto flex h-20 items-center justify-between px-4 md:px-10 lg:h-24 lg:px-12 xl:px-16 2xl:max-w-[1440px] 2xl:px-20"
    >
      <img src="../assets/img/logo.png" class="w-10 lg:w-14" alt="Logo" />

      <!-- MOBILE MENU -->
      <div class="flex lg:hidden">
        <Dialog>
          <DialogTrigger as-child>
            <Menu class="cursor-pointer" />
          </DialogTrigger>

          <DialogContent class="max-w-xs rounded-lg md:max-w-md">
            <DialogHeader>
              <DialogTitle>Wir helfen Ihnen gerne!</DialogTitle>
              <DialogDescription> Hier finden sie uns schnell und einfach. </DialogDescription>
            </DialogHeader>

            <div class="grid gap-2.5">
              <a href="mailto:info@el-reinigung.de">
                <Button type="button" class="w-full">
                  <Mail class="mr-2 w-5" /> info@el-reinigung.de
                </Button>
              </a>
              <a href="tel:+49 174 9524843">
                <Button type="button" class="w-full">
                  <Phone class="mr-2 w-5" /> +49 174 9524843
                </Button>
              </a>
              <a href="https://api.whatsapp.com/send?phone=491749524843" target="_blank">
                <Button class="w-full"><Smartphone class="mr-2 w-5" /> WhatsApp</Button>
              </a>
            </div>
          </DialogContent>
        </Dialog>
      </div>

      <!-- LAPTOP HEADER -->
      <div class="hidden items-center gap-2 lg:flex">
        <TooltipProvider>
          <Tooltip>
            <TooltipTrigger>
              <Button @click="scrollTo('contact-us', 'smooth')" class="text-md font-semibold"
                ><Mail class="w-5"
              /></Button>
            </TooltipTrigger>
            <TooltipContent>
              <p>info@el-reinigung.de</p>
            </TooltipContent>
          </Tooltip>
        </TooltipProvider>
        <TooltipProvider>
          <Tooltip>
            <TooltipTrigger>
              <Button @click="scrollTo('contact-us', 'smooth')" class="text-md font-semibold"
                ><PhoneCall class="w-5"
              /></Button>
            </TooltipTrigger>
            <TooltipContent>
              <p>01523-5884265</p>
            </TooltipContent>
          </Tooltip>
        </TooltipProvider>
        <a href="https://api.whatsapp.com/send?phone=491749524843" target="_blank">
          <Button class="px-4"><Smartphone class="mr-1.5 w-5" />WhatsApp</Button>
        </a>
      </div>
    </div>
  </div>
</template>
