<template>
    <div class="w-full mx-auto py-12 px-4 text-center">
        <div class="w-full text-center space-y-6">
            <h2 class="text-4xl font-semibold">Featured Trip</h2>
            <div class="flex flex-col justify-center items-center gap-3">
                <div class="flex justify-center gap-3">
                    <img src="/Gallery/1.jpeg" alt="">
                    <img src="/Gallery/2.jpeg" alt="">
                </div>
                <div class="flex flex-row-reverse justify-center gap-3">
                    <img src="/Gallery/4.jpeg" alt="">
                    <img src="/Gallery/3.jpeg" alt="">
                </div>
                <div class="flex justify-center gap-3">
                    <img src="/Gallery/5.jpeg" alt="">
                    <img src="/Gallery/6.jpeg" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from "vue";
import Gallery from "vue-gallery";
const images = ref([
    { src: "/Gallery/1.jpeg", alt: "Beach view" },
    { src: "/Gallery/2.jpeg", alt: "Losin lighthouse", text: "LOSIN" },
    { src: "/Gallery/3.jpeg", alt: "Whale shark" },
    { src: "/Gallery/4.jpeg", alt: "Colorful coral reef" },
    { src: "/Gallery/5.jpeg", alt: "Diver near rocks" },
    { src: "/Gallery/6.jpeg", alt: "Diver underwater" }
]);
const index = ref(null);
</script>

<style scoped>
/* ปรับแต่งสไตล์เพิ่มเติมได้ที่นี่ */
</style>