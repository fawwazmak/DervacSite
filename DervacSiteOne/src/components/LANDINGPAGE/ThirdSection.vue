<script>
import { defineComponent } from 'vue';


export default defineComponent({
    props: [],
    components: {},
    data() {
        return {

        }
    }
})
</script>




<template>
    <section class="bg-blue-400 py-12 ">
        <p class="text-center text-2xl font-semibold">Our Services</p>

        <div class="flex md:flex-row flex-col justify-between px-12 py-6">
            <div class="md:w-[30%] md:mb-0 mb-8">
                <img src="../../assets/images/expertImage.jpeg" alt="" class="w-full h-[250px]">
                <p class="pb-4 pt-2 text-white font-medium text-xl md:text-left text-center">Expert IT training Services for Future Success</p>
                <p class="text-center">At our company we believe that continuous learning is the key to staying ahead in the fast-paced world of technology. our comprehensive IT training programs are designed to equip you with the latest industry knowledge and practical skills, empowering you to excel in your career</p>
            </div>

            <div class="md:w-[30%] md:mb-0 mb-8">
                <img src="../../assets/images/accurate.jpeg" alt="" class="w-full h-[250px]">
                <p class="pb-4 pt-2 text-white font-medium text-xl md:text-left text-center">Accurate and Transparent Job/Project Costing Services</p>
                <p  class="text-center">Our job/project costing services provide you with the crucial insights you need to make informed decission and maximize your profitability. We analyze every aspect of your project, from resource allocation to expenses, ensuring you have a clear understanding of the costs involved</p>
            </div>

            <div class="md:w-[30%] md:mb-0 mb-8">
                <img src="../../assets/images/payroll.jpg" alt="" class="w-full h-[250px]">
                <p class="pb-4 pt-2 text-white font-medium text-xl md:text-left text-center">Efficient Payroll Solutions</p>
                <p  class="text-center">Our IT company provides comprehensive payroll services designed to streamline and automate your payroll processes. From calculating employee wages to generating pay stubs, we handle it all with precision and efficiency</p>
            </div>
        </div>
    </section>
</template>



<style></style>