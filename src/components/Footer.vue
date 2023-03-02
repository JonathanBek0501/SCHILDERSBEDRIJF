<template>
    <footer class="bg-brand-black-300">
        <div class="max-w-6xl mx-auto py-14 px-5 md:px-12 lg:px-1.5">
            <div class="grid md:grid-cols-2 gap-5 md:gap-0">
                <div class="grid lg:flex justify-between">
                    <div class="">
                        <h3 class="font-montserrat font-semibold text-lg text-white pb-5">Schildersbedrijf</h3>
                        <p class="lg:max-w-xs font-raleway font-medium text-brand-black-100 pb-6">
                            Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis.
                        </p>
                    </div>
                    <div class="">
                        <h3 class="font-montserrat font-semibold text-lg text-white pb-5">Navigatie</h3>
                        <div class="grid md:grid-cols-2 gap-x-8 gap-y-1.5 font-raleway font-medium text-brand-black-100">
                            <a v-for="(link, index) in navigatie" :key="index" :href="link.href" class="whitespace-nowrap block hover:text-white transition-colors ease-linear">
                                {{ link.title }}
                            </a>
                        </div>
                    </div>
                </div>
                <div class="mt-auto lg:mt-0 max-w-lg w-full md:ml-auto lg:pl-14">
                    <h3 class="font-montserrat font-semibold text-lg text-white pb-5">Services</h3>
                    <div class="grid md:grid-cols-3 gap-1.5 font-raleway font-medium text-brand-black-100">
                        <a v-for="(link, index) in services" :key="index" :href="link.href" class="whitespace-nowrap block hover:text-white transition-colors ease-linear">
                            {{ link.title }}
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script setup>
import { ref } from 'vue'

const navigatie = ref([
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
    {
        title: 'Projecten',
        href: '#',
    },
    {
        title: 'Contact',
        href: '#',
    },
])

const services = ref([
    {
        title: 'Schilderwerk',
        href: '#',
    },
    {
        title: 'Behangen',
        href: '#',
    },
    {
        title: 'Glaswerk',
        href: '#',
    },
    {
        title: 'Repareren',
        href: '#',
    },
    {
        title: 'Herstellen',
        href: '#',
    },
    {
        title: 'Spuiterij',
        href: '#',
    },
    {
        title: 'Offerte',
        href: '#',
    },
    {
        title: 'Projecten',
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