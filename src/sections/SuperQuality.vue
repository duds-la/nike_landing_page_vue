

<template>
    <div id="about-us" class="flex justify-between items-center
    max-lg:flex-col gap-10 w-full max-container">
        <div class="felx flex-1 flex-col ">
            
            <h2 class="font-palanquin capitalize text-4xl font-bold lg:max-w-lg">
                We provide You
                <span class="text-coral-red ">Super </span> 
                <span class="text-coral-red ">Quality</span> Shoes
            </h2>
            <p class="mt-4 lg:max-w-lg info-text">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem, incidunt. Modi, repellendus fuga fugiat ipsum dolorum maiores harum eos, laborum ullam dolore possimus. Quaerat quidem ad delectus incidunt ullam cumque!
            </p>
            <p class="mt-6 lg:max-w-lg info-text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam, culpa. Numquam, corrupti. Natus reprehenderit.
            </p>
            <div class="mt-11">
                <Button label="View Deatails" :iconURL="iconURL"/>
            </div>
        </div>

        <div class="flex-1 flex justify-center items-center">
            <img :src="bigshoe8" alt="" width="570" height="522">
        </div>
    </div>
</template>
<script setup>
import Button from '@/components/Button.vue';
import { shoe8 } from '@/assets/images';
import { ref } from 'vue';

const bigshoe8 = ref(shoe8);
const iconURL = null;
</script>