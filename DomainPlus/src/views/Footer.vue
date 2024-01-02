<script>
import { defineComponent } from 'vue';

export default defineComponent({
    data(){
        return{
            currentYear: new Date().getFullYear(),
        }
    }
})
</script>


<template>
    <div class="bg-black text-white p-12">
        <div class="flex lg:flex-row flex-col lg:items-start items-center lg:text-left text-center lg:justify-between font-bold">
            <div class="lg:w-[20%] w-full">
                <p class="text-2xl mb-4">Address</p>
                
                <div class="flex flex-col gap-y-8">
                    <div class="flex space-x-2 text-[17px]">
                        <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 24 24"><path fill="white" d="m20.665 3.717l-17.73 6.837c-1.21.486-1.203 1.161-.222 1.462l4.552 1.42l10.532-6.645c.498-.303.953-.14.579.192l-8.533 7.701h-.002l.002.001l-.314 4.692c.46 0 .663-.211.921-.46l2.211-2.15l4.599 3.397c.848.467 1.457.227 1.668-.785l3.019-14.228c.309-1.239-.473-1.8-1.282-1.434z"/></svg><p>2 Adaranijo street, opposite Pedro Police Station, Palmgroove, Lagos, Nigeria</p>
                    </div>
                </div>
            </div>


            <div>
                <p class="text-2xl mb-4">Contact Us</p>
                <div class="flex space-x-2 text-[17px] mb-5">
                    <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" viewBox="0 0 24 24"><path fill="white" d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 14H4V8l8 5l8-5v10zm-8-7L4 6h16l-8 5z"/></svg><p>info@domain-plusltd.com</p>
                </div>

                <div class="flex space-x-2 text-[17px]">
                    <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"><path fill="white" d="M4.05 21q-.45 0-.75-.3t-.3-.75V15.9q0-.325.225-.588t.575-.362l3.45-.7q.35-.05.713.063t.587.337L10.9 17q.95-.55 1.8-1.213t1.625-1.437q.825-.8 1.513-1.663t1.187-1.787L14.6 8.45q-.2-.2-.275-.475T14.3 7.3l.65-3.5q.05-.325.325-.563T15.9 3h4.05q.45 0 .75.3t.3.75q0 3.125-1.363 6.175t-3.862 5.55q-2.5 2.5-5.55 3.863T4.05 21Z"/></svg><p>08023121258, 08126290758</p>
                </div>
            </div>


            <div class="flex flex-col gap-y-2 text-left lg:w-fit w-full lg:mt-0 mt-12">
                <p class="lg:text-xl md:text-3xl text-2xl text-center lg:text-left">ABOUT</p>
                <p>WHY DOMAINPLUS</p>
                <p>FIND SERVICES</p>
                <p>FIND SOFTWARE</p>
            </div>

            <!-- <div class="flex flex-col gap-y-10 text-left lg:w-fit w-full lg:mt-0 mt-12">
                <p class="lg:text-xl md:text-3xl text-2xl text-center lg:text-left">ABOUT</p>
                <p>WHY DOMAINPLUS</p>
                <p>CONTACT US</p>
                <p>GLOSSARY</p>
                <p>BLOGS</p>
                <p>HELP CENTER</p>
            </div>

            <div class="flex flex-col gap-y-10 text-left lg:w-fit w-full lg:mt-0 mt-12">
                <p class="lg:text-xl md:text-3xl text-2xl text-center lg:text-left">FOR USER</p>
                <p>RESEARCH METHODOLOGY</p>
                <p>FIND SERVICES</p>
                <p>FIND SOFTWARE</p>
                <p>INSIGHTS</p>
                <p>WRITE A REVIEW</p>
            </div> -->

            <div class="lg:mt-0 mt-12">
                <p class="text-2xl mb-4">Office hour</p>

                <div class="flex space-x-2 text-[17px] mb-0">
                    <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24"><path fill="white" d="M12.5 12.792V8.5q0-.213-.143-.357Q12.213 8 12 8t-.357.143q-.143.144-.143.357v4.379q0 .161.056.3q.056.14.186.271l3.05 3.05q.14.14.345.15q.203.01.363-.15t.16-.354q0-.194-.16-.354l-3-3ZM12 21q-1.663 0-3.118-.626q-1.455-.626-2.543-1.713q-1.087-1.088-1.713-2.543Q4 14.663 4 13q0-1.663.626-3.118q.626-1.455 1.713-2.543q1.088-1.087 2.543-1.713Q10.337 5 12 5q1.663 0 3.118.626q1.455.626 2.543 1.713q1.087 1.088 1.713 2.543Q20 11.337 20 13q0 1.663-.626 3.118q-.626 1.455-1.713 2.543q-1.088 1.087-2.543 1.713Q13.663 21 12 21Zm0-8ZM2.78 7.262q-.159-.16-.159-.354q0-.195.16-.354L5.554 3.78q.14-.14.344-.15q.204-.01.364.15t.16.354q0 .194-.16.353L3.488 7.262q-.14.14-.344.15q-.204.01-.363-.15Zm18.44 0q-.16.16-.355.16q-.194 0-.353-.16l-2.774-2.774q-.14-.14-.15-.344q-.01-.204.15-.363q.16-.16.354-.16q.195 0 .354.16l2.773 2.773q.14.14.15.344q.01.204-.15.364ZM12 20q2.906 0 4.953-2.047T19 13q0-2.906-2.047-4.953T12 6Q9.094 6 7.047 8.047T5 13q0 2.906 2.047 4.953T12 20Z"/></svg><p>Monday - Friday: 09:00 - 18:00</p>
                </div>

                <div class="flex sm:gap-x-6">
                    <div class="bg-blue-800 w-fit rounded-[50%] sm:p-2 p-1 hover:bg-black hover:border hover:border-white transition hover:ease-in-out duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="-7 -2 24 24"><path fill="white" d="M2.046 3.865v2.748H.032v3.36h2.014v9.986H6.18V9.974h2.775s.26-1.611.386-3.373H6.197V4.303c0-.343.45-.805.896-.805h2.254V0H6.283c-4.34 0-4.237 3.363-4.237 3.865z"/></svg>
                    </div>


                    <div class="bg-blue-400 w-fit rounded-[50%] p-2 hover:bg-black hover:border hover:border-white transition hover:ease-in-out duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 256 256"><path fill="white" d="M128 80a48 48 0 1 0 48 48a48.05 48.05 0 0 0-48-48Zm0 72a24 24 0 1 1 24-24a24 24 0 0 1-24 24Zm48-132H80a60.07 60.07 0 0 0-60 60v96a60.07 60.07 0 0 0 60 60h96a60.07 60.07 0 0 0 60-60V80a60.07 60.07 0 0 0-60-60Zm36 156a36 36 0 0 1-36 36H80a36 36 0 0 1-36-36V80a36 36 0 0 1 36-36h96a36 36 0 0 1 36 36ZM196 76a16 16 0 1 1-16-16a16 16 0 0 1 16 16Z"/></svg>
                    </div>


                    <div class="bg-red-600 w-fit rounded-[50%] p-2 hover:bg-black hover:border hover:border-white transition hover:ease-in-out duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 50 50"><path fill="white" fill-rule="evenodd" d="M18 23v4.8h7.9c-.3 2.1-2.4 6-7.9 6c-4.8 0-8.7-4-8.7-8.8s3.9-8.8 8.7-8.8c2.7 0 4.5 1.2 5.6 2.2l3.8-3.7C24.9 12.4 21.8 11 18 11c-7.7 0-14 6.3-14 14s6.3 14 14 14c8.1 0 13.4-5.7 13.4-13.7c0-.9-.1-1.6-.2-2.3H18zm30 0h-4v-4h-4v4h-4v4h4v4h4v-4h4z" clip-rule="evenodd"/></svg>
                    </div>


                    <div class="bg-pink-700 w-fit rounded-[50%] p-2 hover:bg-black hover:border hover:border-white transition hover:ease-in-out duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 20 20"><g fill="white"><path d="M11.5 20a8.5 8.5 0 1 1 0-17a8.5 8.5 0 0 1 0 17Z" opacity=".2"/><path fill-rule="evenodd" d="M1.5 10a8.5 8.5 0 1 0 17 0a8.5 8.5 0 0 0-17 0Zm16 0a7.5 7.5 0 1 1-15 0a7.5 7.5 0 0 1 15 0Z" clip-rule="evenodd"/><path fill-rule="evenodd" d="M6.5 10c0 4.396 1.442 8 3.5 8s3.5-3.604 3.5-8s-1.442-8-3.5-8s-3.5 3.604-3.5 8Zm6 0c0 3.889-1.245 7-2.5 7s-2.5-3.111-2.5-7S8.745 3 10 3s2.5 3.111 2.5 7Z" clip-rule="evenodd"/><path d="m3.735 5.312l.67-.742c.107.096.221.19.343.281c1.318.988 3.398 1.59 5.665 1.59c1.933 0 3.737-.437 5.055-1.19a5.59 5.59 0 0 0 .857-.597l.65.76c-.298.255-.636.49-1.01.704c-1.477.845-3.452 1.323-5.552 1.323c-2.47 0-4.762-.663-6.265-1.79a5.81 5.81 0 0 1-.413-.34Zm0 9.388l.67.74c.107-.096.221-.19.343-.28c1.318-.988 3.398-1.59 5.665-1.59c1.933 0 3.737.436 5.055 1.19c.321.184.608.384.857.596l.65-.76a6.583 6.583 0 0 0-1.01-.704c-1.477-.844-3.452-1.322-5.552-1.322c-2.47 0-4.762.663-6.265 1.789c-.146.11-.284.223-.413.34ZM2 10.5v-1h16v1H2Z"/></g></svg>
                    </div>


                    <div class="bg-violet-600 w-fit rounded-[50%] p-2 hover:bg-black hover:border hover:border-white transition hover:ease-in-out duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 16 16"><path fill="white" d="M4.671 0c.88 0 1.733.247 2.468.702a7.423 7.423 0 0 1 6.02 2.118a7.372 7.372 0 0 1 2.167 5.215c0 .344-.024.687-.072 1.026a4.662 4.662 0 0 1 .6 2.281a4.645 4.645 0 0 1-1.37 3.294A4.673 4.673 0 0 1 11.18 16c-.84 0-1.658-.226-2.37-.644a7.423 7.423 0 0 1-6.114-2.107A7.374 7.374 0 0 1 .529 8.035c0-.363.026-.724.08-1.081a4.644 4.644 0 0 1 .76-5.59A4.68 4.68 0 0 1 4.67 0zm.447 7.01c.18.309.43.572.729.769a7.07 7.07 0 0 0 1.257.653c.492.205.873.38 1.145.523c.229.112.437.264.615.448c.135.142.21.331.21.528a.872.872 0 0 1-.335.723c-.291.196-.64.289-.99.264a2.618 2.618 0 0 1-1.048-.206a11.44 11.44 0 0 1-.532-.253a1.284 1.284 0 0 0-.587-.15a.717.717 0 0 0-.501.176a.63.63 0 0 0-.195.491a.796.796 0 0 0 .148.482a1.2 1.2 0 0 0 .456.354a5.113 5.113 0 0 0 2.212.419a4.554 4.554 0 0 0 1.624-.265a2.296 2.296 0 0 0 1.08-.801c.267-.39.402-.855.386-1.327a2.09 2.09 0 0 0-.279-1.101a2.53 2.53 0 0 0-.772-.792A7.198 7.198 0 0 0 8.486 7.3a1.05 1.05 0 0 0-.145-.058a18.182 18.182 0 0 1-1.013-.447a1.827 1.827 0 0 1-.54-.387a.727.727 0 0 1-.2-.508a.805.805 0 0 1 .385-.723a1.76 1.76 0 0 1 .968-.247c.26-.003.52.03.772.096c.274.079.542.177.802.293c.105.049.22.075.336.076a.6.6 0 0 0 .453-.19a.69.69 0 0 0 .18-.496a.717.717 0 0 0-.17-.476a1.374 1.374 0 0 0-.556-.354a3.69 3.69 0 0 0-.708-.183a5.963 5.963 0 0 0-1.022-.078a4.53 4.53 0 0 0-1.536.258a2.71 2.71 0 0 0-1.174.784a1.91 1.91 0 0 0-.45 1.287c-.01.37.076.736.25 1.063z"/></svg>
                    </div>
                </div>
            </div>
        </div>
        <div class="mt-8">
            <div class="w-full bg-white h-[1px]"></div>
            <p class="text-center mt-2">{{ currentYear }} &copy; DomainPlus Int'l Ltd. All rights reserved | Powered by  <a href="https://dervac.com" target="_blank"><span class="font-[Bimini]">dervac.</span></a></p>
        </div>
    </div>
</template>



<style>
    @font-face {
        font-family: 'Bimini';
        src: url('../assets/bimini/BiminiNormal.ttf') format('truetype');
             /* url('./bimini/BIMINI__.TTF') format('TTF'); */
        /* You can add more formats if needed */
        font-weight: normal;
        font-style: normal;
        /* ./bimini/BiminiNormal.ttf */
    }
</style>