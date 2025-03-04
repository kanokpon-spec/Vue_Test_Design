<template>
    <div class="w-full mx-auto py-12 px-4 text-center">
        <div class="w-full text-center space-y-6">
            <h2 class="text-4xl font-semibold">Featured Trip</h2>

            <swiper :modules="[SwiperAutoplay]" :slides-per-view="1" :space-between="10" :loop="true"
                :autoplay="{ delay: 2500, disableOnInteraction: false }" :breakpoints="{
                    768: { slidesPerView: 2, spaceBetween: 20 },
                    1024: { slidesPerView: 3, spaceBetween: 30 }
                }" class="w-full">
                <swiper-slide v-for="(img, i) in images" :key="i">
                    <div class="w-[343px] h-[343px] mx-auto">
                        <img :src="img.src" :alt="img.alt" class="w-full h-full object-cover rounded-lg">
                    </div>
                </swiper-slide>
            </swiper>
        </div>
    </div>
</template>

<script setup>
import { ref } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay as SwiperAutoplay } from "swiper/modules";
import "swiper/css";

const images = ref([
    { src: "/Gallery/1.jpeg", alt: "Beach view" },
    { src: "/Gallery/2.jpeg", alt: "Losin lighthouse" },
    { src: "/Gallery/3.jpeg", alt: "Whale shark" },
    { src: "/Gallery/4.jpeg", alt: "Colorful coral reef" },
    { src: "/Gallery/5.jpeg", alt: "Diver near rocks" },
    { src: "/Gallery/6.jpeg", alt: "Diver underwater" }
]);
</script>
