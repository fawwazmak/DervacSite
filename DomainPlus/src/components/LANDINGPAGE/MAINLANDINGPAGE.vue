<script>
import { defineComponent } from 'vue';
import FirstSection from './FirstSection.vue';
import SecondSection from './SecondSection.vue';
import ThirdSection from './ThirdSection.vue';
import FourthSection from './FourthSection.vue'; 
import FifthSection from './FifthSection.vue';
import SixthSection from './SixthSection.vue';

export default defineComponent({
    components: {FirstSection, SecondSection, ThirdSection, FourthSection, FifthSection, SixthSection},
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
    <SixthSection />
</template>



<style></style>