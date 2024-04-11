<template>
    <div
      :class="`border-2 rounded-xl ${bigShoeImg === imgURL.bigShoe ? 'border-coral-red' : 'border-transparent'} cursor-pointer max-sm:flex-1`"
      @click="handleClick"
    >
      <div class="flex justify-center items-center bg-gray-200 bg-center bg-cover sm:w-40 sm:h-40 rounded-xl max-sm:p-4">
        <img :src="imgURL.thumbnail" alt="shoe collection" width="127" height="103" class="object-contain" />
      </div>
    </div>
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  const { imgURL, changeBigShoeImage, bigShoeImg } = defineProps(['imgURL', 'changeBigShoeImage', 'bigShoeImg']);
  
  const handleClick = () => {
    console.log(bigShoeImg, imgURL.bigShoe);
    
      changeBigShoeImage(imgURL.bigShoe);
    
  };
  </script>
  