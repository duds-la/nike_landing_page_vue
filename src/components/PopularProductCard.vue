<template>
    <div class="flex flex-1 flex-col w-full max-sm:full">
        <img :src="imgURL" alt="" class="w-[280px] h-[280px]">
        <div class="mt-8 flex justify-start gap-2.5">
            <img :src="star" alt="" width="24" height="24">
            <p class="font-montserrat text-xl leading-normal text-slate-gray">(4.9)</p>
            
        </div>
        <h3 class="mt-2 text-xl leading-normal font-semibold font-palanquin">{{ name }}</h3>
        <p class="mt-2 font-semibold font-montserrat text-coral-red leading-normal">{{ price }}</p>
    </div>
</template>
<script setup>
import { defineProps } from 'vue';
import { star } from '@/assets/icons';

const { imgURL, name, price} = defineProps(['imgURL', 'name', 'price']);
</script>
