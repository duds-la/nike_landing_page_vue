<template>
    <div class="flex justify-center items-center flex-col">
        <img :src="imgURL" :alt="feedback" class="rounded-full object-cover
        w-[120px] h-[120px]">
        <p class="mt-6 max-w-sm text-center info-text">{{ feedback }}</p>
        <div class="mt-3 flex justify-center items-center gap-2.5">
            <img :src="star" alt=""
            width="24" height="24" class="object-contain m-0">
            <p class="text-xl font-montserrat text-slate-gray">({{ rating }})</p>
        </div>
        <h3 class="mt-1 font-palanquin text-3xl text-center font-bold">{{ nome }}</h3>
    </div>
</template>
<script setup>
import { star } from '@/assets/icons';

const { nome, imgURL, rating, feedback} = defineProps(["nome", "imgURL", "rating", "feedback"]);


</script>
