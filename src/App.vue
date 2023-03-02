<script setup>
import Hero from '@/components/Sections/Hero.vue'
import OnsVerhaal from '@/components/Sections/OnsVerhaal.vue'
import Banner from './components/Sections/Banner.vue';
import OnzeProjecten from './components/Sections/OnzeProjecten.vue';
import OnzeServices from './components/Sections/OnzeServices.vue';
import OnzeServices2 from './components/Sections/OnzeServices2.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <main>
    <Hero />
    <OnsVerhaal />
    <OnzeServices />
    <OnzeProjecten />
    <OnzeServices2 />
    <Banner />
  </main>
  <Footer/>
</template>

<style scoped>

</style>
