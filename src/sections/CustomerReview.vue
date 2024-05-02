<template>
    <div class="max-container">
        <h3 class="font-palaquin text-center text-4xl font-bold">
            What Our
            <span class="text-coral-red"> Custumers </span>
            Say?
        </h3>
        <p class="info-text m-auto mt-4 max-w-lg text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt est laudantium sit error. Pariatur fugiat deleniti quod fuga quia cumque consectetur, error.</p>
        <div class="mt-24 flex flex-1 justify-evenly items-center max-lg:flex-col gap-14">

            <ReviewCard v-for="(review, index) in reviews" :key="index" :nome="review.customerName"
            :imgURL="review.imgURL" :rating="review.rating" :feedback="review.feedback"/>

        </div>
    </div>
</template>
<script setup>

import ReviewCard from '../components/ReviewCard.vue';
import { reviews } from "@/constants";

</script>