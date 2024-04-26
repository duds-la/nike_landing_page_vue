<template>
    <div id="products"  class="max-container max-sm:mt-12">
        <div class="felx flex-col justify-start gap-5">
            <h2 class="text-4xl font-palanquin font-bold">Our <span class="text-coral-red"> Popular</span> Products</h2>
            
            <p class="lg: max-w-lg mt-2 font-montserrat text-slate-gray">Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere optio, minus porro necessitatibus quas ad atque error, vero itaque, eveniet culpa quasi.</p>
            <div class="mt-16 grid lg:grid-cols-4 md:grid-cols-3 sm:grid-cols-2 grid-cols-1 sm:gap-4 gap-14">
                <PopularProductCard v-for="(product, index) in products" :key="index" :imgURL="product.imgURL"
                :name="product.name" :price="product.price" />
            </div>
        </div>
    </div>
</template>
<script setup>
import { products } from '@/constants'
import PopularProductCard from '../components/PopularProductCard.vue'

</script>