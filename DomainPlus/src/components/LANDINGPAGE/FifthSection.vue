<script>
import {defineComponent} from 'vue'


export default defineComponent({
    components: {

    },
    data() {
        return {
            partner: 1,
        }
    },
    computed: {
        imageUrl1() {
            return '/images/partner' + this.partner + '.png';   
        },
        imageUrl2() {
            return '/images/partner' + (this.partner + 1) + '.png';   
        },
        imageUrl3() {
            return '/images/partner' + (this.partner + 2) + '.png';   
        },
    },
    mounted () {
        setInterval(this.increasepartner, 9000)
    },
    methods: {
        increasepartner() {
            this.partner += 1;


            if (this.partner >= 10) {
                this.partner = 1
            }
        }
    }
})
</script>


<template>
    <section>
        <div class="py-8">
            <p class="md:text-4xl text-xl text-center text-red-800 font-semibold mb-12 font-mono">Our Partners and Clients</p>
            <div class="flex md:flex-row flex-col md:justify-between md:gap-y-0 gap-y-6 items-center md:w-[70%] md:mx-auto mx-4">
                <img :src="imageUrl1" alt="" class="w-24" />
                <img :src="imageUrl2" alt="" class="w-24" />
                <img :src="imageUrl3" alt="" class="w-24" />
            </div>
        </div>
    </section>
</template>




<style></style>