<script>
import { defineComponent } from 'vue';


export default defineComponent({
    data() {
        return {

        }
    }
})
</script>


<template>
    <div class="main pt-32 flex flex-col items-center pb-12">
        <div>
            <p class="text-gray-600 md:text-6xl text-blue-900 sm:text-3xl text-xl text-center font-medium">Your Complete</p>
            <p class="text-gray-600 md:text-6xl text-blue-900 sm:text-3xl text-xl font-medium">Consulting Partner</p>
        </div>

        <button class="bg-green-500 text-white py-2 md:py-4 md:px-6 px-3 w-fit mt-10 rounded-[5px]">OUR SERVICES</button>
    </div>
</template>



<style>
.main {
    /* background-color: brown; */
    background-image: url(/images/heroSection.jpeg);
    /* height: 70vh; */
    /* width: 100%; */
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: fixed;
}
</style>