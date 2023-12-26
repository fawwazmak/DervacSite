<script>
import { defineComponent } from 'vue';
import FirstSection from './FirstSection.vue';
import SecondSection from './SecondSection.vue';
import ThirdSection from './ThirdSection.vue';
import FourthSection from './FourthSection.vue'; 
import FifthSection from './FifthSection.vue';

export default defineComponent({
    components: {FirstSection, SecondSection, ThirdSection, FourthSection, FifthSection},
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
</template>



<style></style>