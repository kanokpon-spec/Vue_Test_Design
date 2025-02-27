<script setup>
import { ref } from "vue";
const equipment = ref([
    {
        name: "Beanie",
        price: "2,700.00",
        image: "/Equipment/eq1.jpeg"
    },
    {
        name: "Black Pearl - 2 Pieces - Longjohn - 2mm",
        price: "13,500.00",
        image: "/Equipment/eq2.jpeg"
    },
    {
        name: "Jax",
        price: "1,360.00",
        image: "/Equipment/eq3.jpeg"
    },
    {
        name: "MTX-RC Set",
        price: "39,990,00",
        image: "/Equipment/eq4.jpeg"
    }
])
</script>

<template>
    <div class="w-full mx-auto py-12 px-4 text-center">
        <h2 class="text-3xl font-bold">EQUIPMENT</h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 mt-8 text-left">
            <div v-for="(item, index) in equipment" :key="index" class="flex flex-col justify-start items-center p-6">
                <img :src="item.image" alt="">
                <h3 class="text-xl font-semibold text-center pb-3 mt-5 min-h-[70px] text-[#FEC32D]">{{ item.name }}</h3>
                <span class="text-black font-semibold">{{ item.price }}฿</span>
            </div>
        </div>
    </div>
</template>
