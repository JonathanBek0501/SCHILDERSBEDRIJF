<template>
    <!-- Over ons -->
    <div class="relative z-10 max-w-5xl lg:max-w-6xl mx-auto px-5 lg:px-1.5 py-14 lg:pt-0 lg:pb-20 lg:-mt-[92px]">
        <div class="md:flex justify-between items-end space-y-7 md:space-y-0 md:space-x-5">
            <div class="md:w-[55%] lg:w-3/5 font-raleway">
                <h3 class="font-medium pb-3.5">Over ons</h3>
                <h2 class="font-extrabold text-3xl md:text-5xl pb-5 md:pb-8 uppercase">
                    Ons verhaal <span class="text-brand-yellow">.</span>
                </h2>
                <div class="font-medium text-brand-gray-500 space-y-3.5 pb-8">
                    <p>
                        Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
                    </p>
                    <p>
                        Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut.
                    </p>
                </div>
                <div class="grid grid-cols-2 lg:grid-cols-4 gap-5">
                    <!-- Gray Boxes -->
                    <div v-for="(box, index) in boxes" :key="index" class="bg-brand-gray-200 border-b-2 border-brand-gray-300 p-5 space-y-5">
                        <div class="w-10 h-10">
                            <img class="w-full h-full object-cover" :src="box.img" alt="">
                        </div>
                        <p class="font-montserrat font-semibold text-lg">
                            {{ box.title }}
                        </p>
                    </div>
                </div>
            </div>
            <div class="md:w-[45%] lg:w-2/5 md:max-w-sm border-b-2 border-brand-gray-300">
                <form action="#">
                    <div class="flex items-center text-white bg-brand-yellow p-5 lg:px-10 gap-5">
                        <svg class="w-10 h-10 fill-white" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" id="Capa_1" x="0px" y="0px" viewBox="0 0 496 496" style="enable-background:new 0 0 496 496;" xml:space="preserve">
                                <path d="M88,128c13.68,0,24-17.192,24-40s-10.32-40-24-40S64,65.192,64,88S74.32,128,88,128z M88,64c1.992,0,8,8.512,8,24 s-6.008,24-8,24s-8-8.512-8-24S86.008,64,88,64z"></path> <path d="M408,0H88C56.6,0,32,38.656,32,88v184c0,17.673,14.327,32,32,32c5.634-0.033,11.157-1.569,16-4.448V320 c0,17.673,14.327,32,32,32s32-14.327,32-32v-52.448c4.843,2.879,10.366,4.415,16,4.448c17.673,0,32-14.327,32-32v-64h216 c15.824,0,29.912-9.832,40-25.888V168c0,17.673-14.327,32-32,32H288c-23.397,0.043-43.361,16.934-47.28,40H232 c-4.418,0-8,3.582-8,8v24h-8c-4.418,0-8,3.582-8,8v208c0,4.418,3.582,8,8,8h64c4.418,0,8-3.582,8-8V280c0-4.418-3.582-8-8-8h-8 v-24c0-4.418-3.582-8-8-8h-6.864c3.637-14.086,16.317-23.945,30.864-24h128c26.499-0.026,47.974-21.501,48-48V88 C464,38.656,439.4,0,408,0z M240,256h16v16h-16V256z M272,288v192h-48V288H272z M88,16c21.68,0,40,32.968,40,72s-18.32,72-40,72 s-40-32.968-40-72S66.32,16,88,16z M176,240c0,8.837-7.163,16-16,16s-16-7.163-16-16v-24h-16v104c0,8.837-7.163,16-16,16 s-16-7.163-16-16v-64H80v16c0,8.837-7.163,16-16,16s-16-7.163-16-16V150.112C58.088,166.168,72.176,176,88,176h88V240z M408,160 H120.52c16.208-20.408,24.541-45.961,23.48-72c1.061-26.039-7.272-51.592-23.48-72H408c21.68,0,40,32.968,40,72 S429.68,160,408,160z"></path> <rect x="240" y="448" width="16" height="16"></rect>
                            </svg>
                        <div>
                            <p class="font-raleway font-medium"> Contact aanvraag</p>
                            <h2 class="font-montserrat font-bold text-xl">Formulier</h2>
                        </div>
                    </div>
                    <div class="font-roboto font-medium text-brand-400 bg-brand-gray-200 p-5 lg:p-10 space-y-6">
                        <!-- Name -->
                        <div class="border-b border-brand-gray-300">
                            <input type="text" class="w-full bg-brand-gray-200 focus:outline-none border border-transparent focus:border-brand-gray-300 pt-2 pb-2.5 px-4" placeholder="Je naam">
                        </div>
                        <!-- Email -->
                        <div class="border-b border-brand-gray-300">
                            <input type="email" class="w-full bg-brand-gray-200 focus:outline-none border border-transparent focus:border-brand-gray-300 py-2 px-4" placeholder="Email">
                        </div>
                            <!-- Telefon -->
                            <div class="border-b border-brand-gray-300">
                            <input type="text" class="w-full bg-brand-gray-200 focus:outline-none border border-transparent focus:border-brand-gray-300 py-2 px-4" placeholder="Telefon">
                        </div>
                        <div class="group border-b border-brand-gray-300">
                            <textarea class="w-full h-full resize-none bg-brand-gray-200 focus:outline-none border border-transparent  focus:border-brand-gray-300 py-2.5 px-4" name="" id=""  rows="4"  placeholder="Jouw bericht"></textarea>
                        </div>

                        <button type="submit" class="font-raleway min-h-[40px] font-medium w-full text-white hover:text-brand-yellow hover:bg-white bg-brand-yellow transition ease-linear px-6">
                            Aanvraag versturen
                        </button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const boxes = ref([
    {
        title: 'Veiligheid',
        img: '/icons/Veiligheid.svg',
    },
    {
        title: 'Kwaliteit',
        img: '/icons/Kwaliteit.svg',
    },
    {
        title: 'Ervaren',
        img: '/icons/Ervaren.svg',
    },
    {
        title: 'Betaalbaar',
        img: '/icons/Betaalbaar.svg',
    },
])
</script>

<style scoped>

</style>