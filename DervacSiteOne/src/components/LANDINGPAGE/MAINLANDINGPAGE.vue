<script>
import { defineComponent } from 'vue';
import FirstSection from './FirstSection.vue';
import SecondSection from './SecondSection.vue';
import ThirdSection from './ThirdSection.vue';
import FourthSection from './FourthSection.vue'; 
import FifthSection from './FifthSection.vue';
import SixSection from './SixSection.vue';

export default defineComponent({
    components: {FirstSection, SecondSection, ThirdSection, FourthSection, FifthSection, SixSection},
    data(){
        return{
        }
    }
})
</script>


<template>
    <FirstSection />
    <SecondSection />
    <ThirdSection />
    <FourthSection />
    <FifthSection />
    <SixSection />
</template>



<style></style>