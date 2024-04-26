<template>
    <div class="flex justify-wrap items-center max-xl:flex-col-reverse gap-10
    max-container ">
        <div class="flex-1">
            <img :src="offer" width="733" height="687" class="object-contain w-full" alt="">
        </div>
        <div class="felx flex-1 flex-col ">
            
            <h2 class="font-palanquin capitalize text-4xl font-bold lg:max-w-lg">
                <span class="text-coral-red ">Special </span> Offer
            </h2>
            <p class="mt-4 lg:max-w-lg info-text">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem, incidunt. Modi, repellendus fuga fugiat ipsum dolorum maiores harum eos, laborum ullam dolore possimus. Quaerat quidem ad delectus incidunt ullam cumque!
            </p>
            <p class="mt-6 lg:max-w-lg info-text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam, culpa. Numquam, corrupti. Natus reprehenderit.
            </p>
            <div class="mt-11 flex flex-wrap gap-4">
                <Button label="Shop Now" :iconURL="arrowRight"/>
                <Button label="Learn Better" :backgroundColor="bg"
                :boderColor="borde" :textColor="text"/>
            </div>
        </div>
    </div>
</template>
<script setup>
import Button from '@/components/Button.vue';
import {offer} from '../assets/images'
import { arrowRight } from '@/assets/icons';

const bg = 'bg-white';
const borde = 'border-slate-gray';
const text = 'text-slate-gray';
</script>