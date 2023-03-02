<template>
    <!-- Onze services -->
    <div class="bg-brand-gray-200">
        <div class="max-w-6xl mx-auto px-4 py-14 lg:py-20">
            <div class="font-raleway text-center">
                <h3 class="font-medium pb-3.5">Wat kunnen wij doen?</h3>
                <div class="relative z-10">
                    <h2 class="relative z-30 font-extrabold text-3xl md:text-5xl pb-5 md:pb-8 uppercase">
                        Onze services <span class="text-brand-yellow">.</span>
                    </h2>
                    <img class="absolute bottom-7 w-full h-28" src="@/assets/img/Rechthoek4.svg" alt="">
                </div>
                <p class="max-w-2xl mx-auto font-medium pb-8">
                    Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu.
                </p>
                <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-y-8">
                    <div v-for="(item, index) in items" :key="index" class="flex flex-col items-center">
                        <div class="w-10 h-10">
                            <img class="w-full h-full object-cover" :src="item.img" alt="">
                        </div>
                        <p class="font-montserrat font-semibold text-lg pt-5">
                            {{ item.title }}
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const items = ref([
    {
        title: 'Schilderwerk',
        img: '/icons/Veiligheid.svg',
    },
    {
        title: 'Repareren',
        img: '/icons/Repareren.svg',
    },
    {
        title: 'Herstellen',
        img: '/icons/Herstellen.svg',
    },
    {
        title: 'Glaswerk',
        img: '/icons/Glaswerk.svg',
    },
    {
        title: 'Behangen',
        img: '/icons/Behangen.svg',
    },
    {
        title: 'Spuiterij',
        img: '/icons/Spuiterij.svg',
    },
])
</script>

<style scoped>

</style>