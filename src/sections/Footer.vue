<template>
    <footer class="max-container">
        <div class="flex justify-between items-center gap-20
        flex-wrap max-lg:flex-col">
            <div class="flex flex-col items-start">
                <a href="/">
                    <img :src="footerLogo" width="150" height="46">
                </a>
                <p class="mt-6 text-base leading-7 font-montserrat text-white-400 sm:max-w-sm">
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quas cupiditate libero
                </p>
                <div class="flex items-center gap-5 mt-8">
                    <div v-for="(socialMedia, index) in socialMedias" :key="index"
                    class="flex justify-center items-center w-12 h-12 bg-white rounded-full">
                        <img :src="socialMedia.src" alt=""
                        width="24" height="24">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>
<script setup>
import { footerLogo } from "@/assets/images";
import { socialMedia } from "@/constants";

</script>