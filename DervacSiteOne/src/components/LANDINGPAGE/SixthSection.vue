<script>
import {defineComponent} from 'vue'


export default defineComponent({
    components: {

    },
    data() {
        return {
            showing: 1,
        }
    },
    mounted() {
        setInterval(this.changeVariable, 9000)
    },
    methods: {
        changeVariable() {
            this.showing += 1;

            if (this.showing >= 4) {
                this.showing = 1;
            }
        }
    }
})
</script>




<template>
    <section class="testimonials py-8 md:px-24 flex flex-col items-center">
        <p class="text-center text-white text-3xl font-medium">Our Testimonials</p>
        <div class="mt-10">
            <div v-show="showing == 1" class="text-black flex flex-col items-center">
                <img src="/images/testimony1.jpeg" alt="witness Image" class="h-28 w-28 rounded-[50%] mb-4">
                <p class="font-medium  text-2xl">Kolade Ishola</p>
                <p class="text-gray-600 md:mb-5">Ceo Draft</p>

                <p class="px-16 text-center quote-mark"> <span class="text-2xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore perferendis, totam aperiam laboriosam, odio sequi deserunt dolores voluptas, fuga qui temporibus nobis molestiae dicta repellendus molestias et labore eveniet! Accusamus</span> </p>
            </div>

            <div v-show="showing == 2" class="text-black flex flex-col items-center">
                <img src="/images/testimony2.jpeg" alt="witness Image" class="h-28 w-28 rounded-[50%] mb-4">
                <p class="font-medium  text-2xl">Adeyemo Cave</p>
                <p class="text-gray-600 md:mb-5">Manager Fasy</p>

                <p class="px-16 text-center quote-mark"> <span class="text-2xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore perferendis, totam aperiam laboriosam, odio sequi deserunt dolores voluptas, fuga qui temporibus nobis molestiae dicta repellendus molestias et labore eveniet! Accusamus</span> </p>
            </div>

            <div v-show="showing == 3" class="text-black flex flex-col items-center">
                <img src="/images/testimony3.jpeg" alt="witness Image" class="h-28 w-28 rounded-[50%] mb-4">
                <p class="font-medium  text-2xl">Cyntia Cole</p>
                <p class="text-gray-600 md:mb-5">Director Holics</p>

                <p class="px-16 text-center quote-mark"> <span class="text-2xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore perferendis, totam aperiam laboriosam, odio sequi deserunt dolores voluptas, fuga qui temporibus nobis molestiae dicta repellendus molestias et labore eveniet! Accusamus</span> </p>
            </div>
        </div>

        <!-- The dots showing the stage of the testimonials  -->
        <div class="flex space-x-4 mt-8">
            <div class="w-4 h-4 rounded-[50%] border border-red-800 border-[2px]" :class="showing == 1 ? 'bg-blue-800' : '' " @click="this.showing = 1"></div>
            <div class="w-4 h-4 rounded-[50%] border border-red-800 border-[2px]" :class="showing == 2 ? 'bg-blue-800' : '' " @click="this.showing = 2"></div>
            <div class="w-4 h-4 rounded-[50%] border border-red-800 border-[2px]" :class="showing == 3 ? 'bg-blue-800' : '' " @click="this.showing = 3"></div>
        </div>
    </section>
</template>





<style>
    .testimonials {
        background-image: url(/images/testimonialBackground.jpg);
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;
    }
    .quote-mark:before {
        content: "\201C";
        box-sizing: border-box;
        font-size: 40px;
        color: rgb(179, 117, 117);
    }
    .quote-mark:after {
        content: "\201D";
        box-sizing: border-box;
        font-size: 40px;
        color: rgb(179, 117, 117);
    }
    @media (max-width: 640px) {
        .quote-mark:before {
            font-size: 70px;
            color: rgb(179, 117, 117);
        }
        .quote-mark:after {
            font-size: 70px;
            color: rgb(179, 117, 117);
        }
    }
</style>