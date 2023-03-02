<template>
    <!--  Onze projecten -->
    <div class="max-w-6xl mx-auto px-4 py-14 lg:py-20 text-center">
        <div class="font-raleway pb-8">
            <h3 class="font-medium pb-3.5">Afgerond werk van ons</h3>
            <div class="relative z-10">
                <h2 class="relative z-30 font-extrabold text-3xl md:text-5xl uppercase">
                    Onze projecten <span class="text-brand-yellow">.</span>
                </h2>
                <img class="absolute bottom-0 w-full h-28" src="@/assets/img/Rechthoek4.svg" alt="">
            </div>
        </div>
        <div class="grid lg:grid-cols-3 gap-8 pb-10">
            <div v-for="(card, index) in cards" :key="index" class="relative h-[313px]">
                <div class="absolute inset-0 w-full h-full bg-project">
                </div>
                <!-- <img class="w-full h-full object-cover" src="" alt=""> -->
                <div class="absolute bottom-8 left-8 text-start">
                <p class="font-raleway font-medium text-brand-yellow pb-5">{{ card.title }}</p>
                <h2 class="font-montserrat font-semibold text-lg text-white">{{ card.subTitle }}</h2>
                </div>
            </div>
        </div>
        <a href="#" class="inline-block text-white lg:hover:text-brand-yellow bg-brand-yellow lg:hover:bg-white transition ease-linear leading-4 py-4 px-5">
            Meer projecten laten zien
        </a>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const cards = ref([
    {
        title: 'Wageningen, Gelderland',
        subTitle: 'Woonkamer schilderwerk',
        img: '',
    },
    {
        title: 'Ede, Gelderland',
        subTitle: 'Glaswerk vervangen',
        img: '',
    },
    {
        title: 'Bennekom, Gelderland',
        subTitle: 'Woonkamer schilderwerk',
        img: '',
    },
])
</script>

<style scoped>

</style>