<template>
  <div>
    <button class="flex justify-center items-center gap-2 px-7 py-2 border font-montserrat
      text-lg leading-none bg-coral-red rounded-full text-white border-coral-red">
      {{ label }}
      <img :src="iconURL" alt="icon" class="ml-2 rounded-full w-5 h-5">
    </button>
    
  </div>
</template>

<script setup>


const props = defineProps({
  label: String,
  iconURL: String
});

</script>