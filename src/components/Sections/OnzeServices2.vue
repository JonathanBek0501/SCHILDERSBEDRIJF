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
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-10 text-start gap-y-8">
                    <div v-for="(item, index) in items" :key="index" class="relative bg-white px-8 pb-8 z-10">
                        <div class="relative z-10 flex items-end mb-5 md:mb-10">
                            <span class="w-10 h-10 p-2.5 text-white bg-brand-yellow text-center font-montserrat font-bold text-4xl leading-8 uppercase">"</span>
                            <div class="w-16 h-16">
                                <img class="w-full h-full object-cover" :src="item.img" alt="">
                            </div>
                        </div>
                        <p class="font-raleway font-medium text-brand-gray-500">
                            {{ item.description }}
                        </p>
                        <div class="absolute top-0 inset-x-0 bg-brand-gray-200 h-10 z-0"></div>
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
        description: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget, penatibus et magnis. Cum sociis natoque penatibus.',
        img: '/img/service-1.jpeg',
    },
    {
        description: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget, penatibus et magnis. Cum sociis natoque penatibus.',
        img: '/img/service-2.jpeg',
    },
    {
        description: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget, penatibus et magnis. Cum sociis natoque penatibus.',
        img: '/img/service-3.jpeg',
    },
])
</script>

<style scoped>

</style>