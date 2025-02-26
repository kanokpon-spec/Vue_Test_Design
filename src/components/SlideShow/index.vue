<template>
    <div class="slick-container">
        <div><img src="/image/image1.jpeg" alt="Slide 1" /></div>
        <div><img src="/image/image2.jpeg" alt="Slide 2" /></div>
        <div><img src="/image/image3.jpeg" alt="Slide 3" /></div>
    </div>
</template>

<script>
import $ from 'jquery'; // นำเข้า jQuery
import 'slick-carousel/slick/slick.css'; // นำเข้า CSS ของ Slick
import 'slick-carousel/slick/slick-theme.css'; // นำเข้า CSS สำหรับธีม
import 'slick-carousel'; // นำเข้า JavaScript ของ Slick

export default {
    mounted() {
        this.$nextTick(() => {
            $('.slick-container').slick({
                slidesToShow: 1, // แสดงเพียง 1 ภาพ
                slidesToScroll: 1, // เลื่อน 1 ภาพ
                autoplay: true, // เลื่อนอัตโนมัติ
                autoplaySpeed: 2000, // ความเร็วในการเลื่อนอัตโนมัติ
                // centerMode: true, // โหมดกลาง เพื่อแสดงภาพข้างๆ
                // centerPadding: '40px', // เพิ่ม padding ข้างๆ ภาพ
                arrows: true, // แสดงปุ่ม navigation
                dots: true, // แสดง pagination
                infinite: true, // เลื่อนวนไปเรื่อยๆ
            });
        });
    },
};
</script>

<style scoped>
.slick-container {
    width: 100%;
    height: 100%;
}

.slick-container img {
    width: 100%;
    height: auto;
    /* margin: 0 15px; */
}
</style>