<script>
import { defineComponent } from 'vue';
import elementStore from '../stores/counter'


export default defineComponent({
    data(){
        return {
            isHidden: false,
            drop: elementStore().$state.drop,
        }
    },
    mounted() {
        window.addEventListener('scroll', this.handleScroll);
    },
    destroyed() {
        window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
        handleScroll() {
            var scrollPosition = window.scrollY;

            var hideHeight = 200;
            this.isHidden = scrollPosition >= hideHeight;
        },
        toggleDrop() {
            this.drop = !this.drop;
        }
    }
})
</script>



<template>
    <div>
        <div class="bg-blue-900 w-full md:h-8 relative py-1" :class="isHidden ? 'hidden' : 'block'" >
            <div class="flex md:gap-x-12 gap-x-3 w-fit md:absolute md:right-4 md:px-0 px-4 md:text-base text-xs">
                <div class="sm:font-semibold flex md:gap-x-2">
                    <p class="md:text-gray-400 text-white">EMAIL US:</p>
                    <a href="http://" target="_blank" class="text-white">info@hub.com</a>
                </div>
                <div class="bg-black h-6 w-[2px] md:block hidden"></div>
                <div class="sm;font-semibold flex md:gap-x-2">
                    <p class="md:text-gray-400 text-white">CALL US NOW:</p>
                    <a href="http://" target="_blank" class="text-white">09084563778</a>
                </div>
            </div>
        </div>
        <div class="flex justify-between items-center sm:px-12 px-4 py-4" :class="isHidden ? 'bg-black' : 'bg-white'">
            <div class="flex items-center ">
                <img src="../assets/images/logo.png" alt="logo" class="md:w-[40px] w-[30px]">
            </div>

            <ul class="flex md:flex-row md:relative left-0 md:bg-none  md:p-0 md:space-y-0 md:top-0  md:h-fit md:justify-between md:items-center md:gap-x-8 font-semibold" :class="drop? 'flex-col absolute bg-white z-20 p-4 space-y-6 top-[100px] h-screen ' : 'hidden md:flex'" >
                <li :class="isHidden ? 'text-white' : 'text-blue-800' ">HOME</li>
                <li :class="isHidden ? 'text-white' : 'text-blue-800' ">ABOUT US</li>
                <li :class="isHidden ? 'text-white' : 'text-blue-800' ">SERVICES</li>
                <li :class="isHidden ? 'text-white' : 'text-blue-800' ">BLOG</li>
                <li :class="isHidden ? 'text-white' : 'text-blue-800' ">CONTACT US</li>
            </ul>

            <div class="md:hidden" @click="toggleDrop()">
                <svg v-if="!drop" xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32"><path fill="none" stroke="blue" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h22M5 16h22M5 24h22"/></svg>


                <svg v-else xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"><path fill="blue" d="m12 13.4l-4.9 4.9q-.275.275-.7.275t-.7-.275q-.275-.275-.275-.7t.275-.7l4.9-4.9l-4.9-4.9q-.275-.275-.275-.7t.275-.7q.275-.275.7-.275t.7.275l4.9 4.9l4.9-4.9q.275-.275.7-.275t.7.275q.275.275.275.7t-.275.7L13.4 12l4.9 4.9q.275.275.275.7t-.275.7q-.275.275-.7.275t-.7-.275L12 13.4Z"/></svg>
            </div>
        </div>

        <div class="bg-gray-200 opacity-20 w-screen absolute h-screen" v-show="drop" @click="toggleDrop()"></div>
    </div>
</template>


<style>
@font-face {
        font-family: 'Bimini';
        src: url('../assets/bimini/BiminiNormal.ttf') format('truetype');
             /* url('./bimini/BIMINI__.TTF') format('TTF'); */
        /* You can add more formats if needed */
        font-weight: normal;
        font-style: normal;
        /* ./bimini/BiminiNormal.ttf */
    }
</style>