<template>
  <div>
    <button :class="[
      'flex justify-center items-center gap-2 px-7 py-2 border font-montserrat text-lg leading-none rounded-full',
      backgroundColor ? backgroundColor : 'bg-coral-red',
      textColor ? textColor : 'text-white',
      boderColor   ? borderColor : 'border-coral-red'
    ]">
      {{ label }}
      <img v-if="iconURL" :src="iconURL" alt="icon" class="ml-2 rounded-full w-5 h-5">
    </button>

  </div>
</template>

<script setup>


const props = defineProps({
  label: String,
  iconURL: String,
  backgroundColor: String,
  boderColor: String,
  textColor: String
});

</script>