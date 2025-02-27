<script setup>
import SlideShow from '../components/SlideShow/index.vue'
import BannerBeginner from '../components/BannerBeginner/index.vue'
import QA from '../components/QA/index.vue'
import FeaturedTrip from '../components/FeaturedTrip/index.vue'
import Equipment from '../components/Equipment/index.vue'
</script>

<template>
    <div class="overflow-hidden">
        <SlideShow />
        <div class="container mx-auto">
            <BannerBeginner />
            <QA />
            <FeaturedTrip />
            <Equipment />
        </div>
    </div>
</template>

<style scoped>
/* หากต้องการปรับแต่งเพิ่มเติมนอกเหนือจาก Tailwind CSS สามารถเพิ่ม CSS ที่นี่ได้ */
</style>