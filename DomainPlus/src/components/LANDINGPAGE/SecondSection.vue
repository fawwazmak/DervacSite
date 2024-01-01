<script>
import {defineComponent} from 'vue';


export default defineComponent({

})
</script>


<template>
    <div class="bg-white flex lg:flex-row flex-col lg:justify-between md:px-24 sm:px-10 px-4">
        <div class="py-12 lg:w-[60%] lg:text-left text-center">
            <p class="text-2xl text-[#224c75] font-bold">Your Technical Support</p>
            <p class="font-medium text-gray-500">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla distinctio itaque voluptate laboriosam praesentium maxime inventore ullam deleniti, corrupti eos esse qui dolor impedit facere ipsum quidem unde numquam culpa! Vero, illum consequatur. Deserunt nesciunt soluta asperiores, harum laboriosam placeat animi aliquid. Numquam soluta illo magnam reprehenderit? Consequuntur voluptas obcaecati possimus similique cum est quam, veniam asperiores temporibus neque quis dolores error laborum eaque consequatur! Fuga expedita quo in dolores.</p>
        </div>

        <div>
            <form action="/" method="post" class="bg-blue-100 p-8">
                <label class="" for="name">NAME*</label>
                <input type="text" class="block mb-6 lg:w-[300px] w-full" id="name" required>

                <label class="" for="email">EMAIL*</label>
                <input type="text" class="block mb-6 lg:w-[300px] w-full" id="email" required>


                <label class="" for="telephone">PHONE*</label>
                <input type="text" class="block mb-6 lg:w-[300px] w-full" id="telephone" required>


                <label class="" for="service">SERVICE</label>
                <input type="number" class="block mb-6 lg:w-[300px] w-full" id="service" >

                <label class="" for="comment">MESSAGE*</label>
                <textarea name="message" class="block mb-6 lg:w-[300px] w-full" id="comment" cols="30" rows="10"></textarea>


                <button type="submit" class="w-full bg-green-400 text-white font-medium">SEND</button>
            </form>
        </div>
    </div>
</template>



<style>
input:focus, textarea {
        border: none;
        outline: none;
}

input, textarea {
    background-color: transparent;
    border-bottom: 1px solid gray;
}
</style>