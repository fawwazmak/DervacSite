<script>
import {defineComponent} from 'vue'


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
    <section class="project">
        <div class="py-8">
            <div class="flex items-center md:gap-x-2 w-fit mx-auto">
                <div class="bg-white md:h-2 h-[2px] sm:w-20 w-8"></div>
                <p class="text-white md:text-3xl text-sm font-semibold text-center">Latest Project</p>
                <div class="bg-white md:h-2 h-[2px] sm:w-20 w-8"></div>
            </div>


            <div class="grid md:grid-cols-3 md:space-x-6 space-y-6 py-8 md:px-8 px-2">
                <div class="bg-slate-700 hover:bg-red-600 w-fit p-4 relative rounded-[10px]">
                    <img src="../../assets/images/insideProject1.jpeg" alt="" class="w-full h-[280px] rounded">
                    <p class="text-gray-500 mt-6">March 4, 2017</p>
                    <p class="text-white hover:text-red-800">Standard dummy text ever since the 1500s, when an unknown printer took a galley of type and ....</p>
                </div>

                <div class="bg-slate-700 hover:bg-red-600 w-fit p-4 relative rounded-[10px]">
                    <img src="../../assets/images/insideProject2.jpeg" alt="" class="w-full h-[280px] rounded">
                    <p class="text-gray-500 mt-6">March 3, 2017</p>
                    <p class="text-white hover:text-red-800">The provide access to client focused manufactured products best of bread promote cutting edge innovation ....</p>
                </div>


                <div class="bg-slate-700 hover:bg-red-600 w-fit p-4 relative rounded-[10px]">
                    <img src="../../assets/images/insideProject3.jpeg" alt="" class="w-full h-[280px] rounded">
                    <p class="text-gray-500 mt-6">March 3, 2017</p>
                    <p class="text-white hover:text-red-800">Iniatiate technology through effective innovative deply team driven leadership strategic best practices....</p>
                </div>


                <div class="bg-slate-700 hover:bg-red-600 w-fit p-4 relative rounded-[10px]">
                    <img src="../../assets/images/insideProject1.jpeg" alt="" class="w-full h-[280px] rounded">
                    <p class="text-gray-500 mt-6">March 4, 2017</p>
                    <p class="text-white hover:text-red-800">Standard dummy text ever since the 1500s, when an unknown printer took a galley of type and ....</p>
                </div>


                <div class="bg-slate-700 hover:bg-red-600 w-fit p-4 relative rounded-[10px]">
                    <img src="../../assets/images/insideProject2.jpeg" alt="" class="w-full h-[280px] rounded">
                    <p class="text-gray-500 mt-6">March 3, 2017</p>
                    <p class="text-white hover:text-red-800">The provide access to client focused manufactured products best of bread promote cutting edge innovation ....</p>
                </div>


                <div class="bg-slate-700 hover:bg-red-600 w-fit p-4 relative rounded-[10px]">
                    <img src="../../assets/images/insideProject3.jpeg" alt="" class="w-full h-[280px] rounded">
                    <p class="text-gray-500 mt-6">March 3, 2017</p>
                    <p class="text-white hover:text-red-800">Iniatiate technology through effective innovative deply team driven leadership strategic best practices....</p>
                </div>
            </div>            
        </div>
    </section>
</template>




<style>
    .project {
        background-image: url(../../assets/images/latestProjectBackground.jpeg);
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;
    }
</style>