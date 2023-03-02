<template>
    <header>
        <!-- Navigation -->
        <div class="relative border-b border-white/25 z-10">
            <div class="max-w-6xl text-white flex items-center justify-between md:justify-start md:gap-x-20 lg:gap-x-24 mx-auto px-6 lg:px-1.5 pb-3.5 md:pb-0 pt-3.5">
                <a href="#" class="flex items-center space-x-2.5 md:space-x-5">
                    <div class="w-10 h-10">
                        <img class="w-full h-full object-cover" src="@/assets/logo.svg" alt="">
                    </div>
                     <p class="font-montserrat font-bold text-xl text-white uppercase">
                        Schildersbedrijf
                        <span class="text-brand-yellow">.</span>
                    </p>
                </a>

                <nav class="font-montserrat font-semibold hidden md:flex items-center space-x-5">
                    <a v-for="(link, index) in links" :key="index" :href="link.href" :class="index == 0 ? 'border-brand-yellow' : 'border-transparent'" class="focus:border-brand-yellow border-b-2 lg:hover:border-brand-yellow py-6 transition ease-linear">
                    {{ link.title }}
                    </a>
                </nav>

                <button @click="toggleMenu()" class="md:hidden border border-white p-1">
                    <svg :class="menuActive == true ? 'hidden' : 'block'" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                    </svg>

                    <svg :class="menuActive == true ? 'block' : 'hidden'" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                    </svg>
                </button>
            </div>
        </div>

        <!-- mobile menu -->
        <div :class="menuActive == true ? 'max-h-full' : 'max-h-0 overflow-hidden'" id="mobileMenu" class="transition-all ease-in-out duration-300 fixed top-[68px] left-0 w-full h-full bg-white font-montserrat z-50">
            <a v-for="(link, index) in links" :key="index" :href="link.href" :class="index == 0 ? 'bg-brand-yellow text-white' : 'bg-transparent'" class="block transition-all ease-in-out hover:bg-brand-yellow hover:text-white py-2.5 px-5">
                {{ link.title }}
            </a>
        </div>
    </header>
</template>

<script setup>
import { ref } from 'vue'

const menuActive = ref(false)

const toggleMenu = () => {
      menuActive.value = !menuActive.value;
      
      if (menuActive.value) {
        document.body.classList.add("overflow-hidden");
      } else {
        document.body.classList.remove("overflow-hidden");
      }
    }

const links = ref([
    {
        title: 'Home',
        href: '#',
    },
    {
        title: 'Losse dienst',
        href: '#',
    },
    {
        title: 'Over ons',
        href: '#',
    },
    {
        title: 'Contact',
        href: '#',
    },
])

</script>

<style scoped>

</style>