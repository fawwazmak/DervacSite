<script>
import { defineComponent } from 'vue';


export default defineComponent({

})
</script>



<template>
    <div>
        <div class="bg-blue-900 w-full h-8 relative py-1">
            <div class="flex gap-x-12 w-fit absolute right-4">
                <div class="font-semibold flex gap-x-2">
                    <p class="text-gray-400">EMAIL US:</p>
                    <a href="http://" target="_blank" class="text-white">info@hub.com</a>
                </div>
                <div class="bg-black h-6 w-[2px]"></div>
                <div class="font-semibold flex gap-x-2">
                    <p class="text-gray-400">CALL US NOW:</p>
                    <a href="http://" target="_blank" class="text-white">09084563778</a>
                </div>
            </div>
        </div>
        <div class="flex justify-between items-center bg-white px-12 py-4">
            <div class="flex items-center ">
                <img src="../assets/images/dervac_logo.png" alt="logo" class="w-[40px]">
                <p class="font-[Bimini] text-[#224c75] text-2xl">dervac<span class="text-red-600">Hub</span></p>
            </div>

            <ul class="flex justify-between items-center gap-x-8 font-semibold text-blue-800">
                <li>HOME</li>
                <li>ABOUT US</li>
                <li>SERVICES</li>
                <li>BLOG</li>
                <li>CONTACT US</li>
            </ul>
        </div>
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