<template>
    <div class="relative w-full h-full bg-cover bg-no-repeat">
        <div class="absolute bg-layer-black left-0 top-0 w-full h-full z-10"></div>
        <img class="absolute inset-0 w-full h-full object-cover z-0" src="@/assets/img/hand-paint-paint-roller.jpg" alt="">
        <Header/>
        <!--  Hero-->
        <div class="relative font-raleway text-white text-center pt-24 lg:pt-36 pb-32 lg:pb-44 z-10 px-5">
            <p class="pb-5">Welkom bij</p>
            <h2 class="font-extrabold text-3xl md:text-5xl pb-5 md:pb-8 uppercase">
                Schildersbedrijf <span class="text-brand-yellow">.</span>
            </h2>
            <p class="pb-5 md:pb-8">
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus,
                <br class="hidden sm:inline-block">
                 luctus nec ullamcorper mattis, pulvinar dapibus leo.
            </p>
            <div class="font-medium space-x-5">
                <a href="#" class="inline-block text-white lg:hover:text-brand-yellow bg-brand-yellow lg:hover:bg-white transition ease-linear leading-4 py-4 px-5">
                    Meer over ons
                </a>
                <a href="#" class="inline-block text-black lg:hover:text-white bg-white lg:hover:bg-brand-yellow transition ease-linear leading-4 py-4 px-5">
                    Kom in contact
                </a>
            </div>
        </div>
    </div>
</template>

<script setup>
import Header from '@/components/Header.vue'
</script>

<style scoped>

</style>