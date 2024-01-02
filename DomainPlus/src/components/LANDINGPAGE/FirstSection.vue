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
        <section class="relative bg-blue-400">
            <div class="main pt-32 flex flex-col items-center pb-28">
                <div>
                    <p class="text-gray-600 md:text-6xl text-blue-900 sm:text-3xl text-xl text-center font-medium">Your Complete</p>
                    <p class="text-gray-600 md:text-6xl text-blue-900 sm:text-3xl text-xl font-medium">Consulting Partner</p>
                </div>

                <button class="bg-green-500 text-white py-2 md:py-4 md:px-6 px-3 w-fit mt-10 rounded-[5px]">OUR SERVICES</button>
            </div>


            <div class="flex md:flex-row flex-col-reverse md:w-[87%] md:mx-auto relative md:top-[-70px] md:gap-x-4">
                <div class="p-4 md:rounded-[6px] bg-[#031f49] text-white md:text-left text-center">
                    <p class="text-3xl font-bold">Your Technical Support</p>
                    <p class="mt-8">Domain-Plus Int'l Limited is leading ICT counsultancy and Training Provider in Nigeria. We assist our clients in achieving significant improvements in operating performance via state-of-the-art automation. </p>

                    <div class="mx-auto w-fit mt-6 bg-gray-500 px-4 py-2 rounded-[18px] cursor-pointer">Contact Us</div>
                </div>

                
                <div class="p-4 md:rounded-[6px] bg-white text-center shadow-2xl">
                    <p class="text-2xl text-[#224c75] font-semibold">Fleet Management & Tracking</p>
                    <p class="mt-8 text-gray-500">Harness the power of connected systems allowing you to make informed decisions effortlessly.</p>
                </div>

                <div class="p-4 md:rounded-[6px] bg-white text-center shadow-2xl">
                    <p class="text-xl text-[#224c75] font-semibold">Payroll & Human Resource Management</p>
                    <p class="mt-8 text-gray-500"> Let's transform your HR processes for a brighter future!</p>
                </div>


                <div class="p-4 md:rounded-[6px] bg-white text-center shadow-2xl">
                    <p class="text-2xl text-[#224c75] font-semibold">Finance and Accounting</p>
                    <p class="mt-8 text-gray-500">Let us empower your growth in your financial landscape.</p>
                </div>
            </div>
        </section>
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