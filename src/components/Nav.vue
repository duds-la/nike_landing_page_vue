<template>
    <header class="padding-x py-8 absolute z-10 w-full ">
        <nav class="flex justify-between items-center max-container ">
            <a href="/">
                <img :src="headerLogo" alt="Logo" width="130" height="29" />
            </a>
            <ul class="flex-1 flex justify-center items-center gap-16 max-lg:hidden">
                <li v-for="(link, index) in navLinksSrc" :key="index">
                    <a class="font-montserrat
                    leading-normal text-lg text-slate-gray" 
                    :href="link.href">{{ link.label }}
                </a>
                </li>
            </ul>
            <div class="hidden max-lg:block">
                <img :src="hamburger" alt="hamburguer" width="24" height="24">
            </div>
        </nav>
    </header>
</template>

<script setup>
import { hamburger } from "@/assets/icons";
import { headerLogo } from "@/assets/images";
import { navLinks } from "../constants";

const headerLogoSrc = headerLogo;
const hamburgerSrc = hamburger;
const navLinksSrc = navLinks;

</script>
