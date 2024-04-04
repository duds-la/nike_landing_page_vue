<template>
  <div class="relative">
    <Nav />
    <section class="xl:padding-1 wide:padding-r padding-b">
      <Hero />
    </section>
    <section class="padding ">
      <PopularProducts />
    </section>
    <section class="padding ">
      <SuperQuality />
    </section>
    <section class="padding-x py-10">
      <Services />
    </section>
    <section class="padding ">
      <SpecialOffer />
    </section>
    <section class="bg-pale-blue padding  ">
      <CustomerReview />
    </section>
    <section class="padding-x sm:py-32 py-16 w-full ">
      <Subscribe />
    </section>
    <section class="bg-black padding-x padding-t pb-8  ">
      <Footer />
    </section>
  </div>
</template>
<script setup>
import {Hero, CustomerReview, Footer, PopularProducts, Services,
SpecialOffer, Subscribe, SuperQuality} from './sections/index';
import Nav from './components/Nav.vue'

</script>

