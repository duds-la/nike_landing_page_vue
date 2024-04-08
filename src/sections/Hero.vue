<template>
    <section id="home" class="w-full flex xl:flex-row flex-col justify-center 
    min-h-screen gap-10 max-container">
        <div class="relative xl:w-2/5 flex flex-col justify-center items-start 
        w-full max-xl:padding-x pt-28">
            <p class="text-xl font-montserrat text-coral-red">Our Summer Collection</p>
            <h1 class="mt-10 font-palanquin text-8xl max-sm:text-[72px] max-sm:leading-[82] font-bold">
                <span class="xl:bg-white xl:whitespace-nowrap relative z-10
                pr-10">The New Arrival</span>
                <br />
                <span class="text-coral-red inline-block mt-3">Nike</span> Shoes
            </h1>
            <p class="font-montserrat text-slate-gray text-lg leading-8 mt-6 mb-14 sm:max-w-sm">Discover stylish Nike
                arrivals,
                quality comfort, and innovattion for your active life.
            </p>
            <Button label="Shop Now" :iconURL=iconarrowRight />
            <div class="flex justify-start items-start flex-wrap w-full
            mt-20 gap-16 ">
                <div v-for="(item, index) in statistics" :key="index">
                    <p class="text-4xl font-palanquin font-bold">{{ item.value }}</p>
                    <p class="left-7 font-montserrat text-slate-gray">{{ item.label }}</p>
                </div>
            </div>
        </div>
        <div class="relative flex-1 flex justify-center items-center xl:min-h-screen max-xl:py-40 bg-primary bg-hero
         bg-cover bg-center ">
            <img :src=imageBigShoe1 alt="" 
            width="610" height="500" class="object-contain relative z-10"/>
        </div>
        <div>
            
        </div>
    </section>
</template>
<script setup>
import { statistics } from '@/constants';
import { arrowRight } from '@/assets/icons'
import Button from '../components/Button.vue'
import {bigShoe1} from '@/assets/images' 

const iconarrowRight = arrowRight;
const imageBigShoe1 = bigShoe1;
</script>