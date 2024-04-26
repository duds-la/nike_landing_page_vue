<template>
    <div class="max-container flex justify-center flex-wrap gap-9">
        <ServiceCard v-for="(service, index) in services" :key="index" :imgURL="service.imgURL"
        :label="service.label" :subtext="service.subtext" />
    </div>
</template>
<script setup>
import { services } from '@/constants'
import ServiceCard from '../components/ServiceCard.vue'

</script>