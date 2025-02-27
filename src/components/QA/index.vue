<script setup>
import { ref } from "vue";

const qnaList = ref([
    {
        questionEn: "HOW ABOUT SHARK?",
        questionTh: "ฉลามจะกัดเรามั้ย",
        content: `จะเจอฉลามสักตัวไม่ใช่เรื่องง่ายนัก เพราะสมัยนี้ หายากเหลือเกินฉลามจะกินอาหารที่ขนาดเล็ก กว่าตัวมันประมาณ 3-4 เท่า และมนุษย์ไม่ใช่ อาหารของฉลามฉลามพันธุ์บางสายพันธุ์เท่านั้น ที่จะจู่โจมคนนั้น ส่วนใหญ่เกิดจากความเข้าใจผิด ส่วนใหญ่อาศัยในน้ำเย็นส่วนใหญ่ที่พบเจอจะเป็น Reef Shark ฉลามประเภทนี้กลัวคนมาก ถ้าเรา เข้าไปใกล้ นิดเดียวเค้าก็จะว่ายหนีไป`
    },
    {
        questionEn: "HOW DEEP?",
        questionTh: "ดํากับลึกแค่ไหน",
        content: `สำหรับการคอร์สดำน้ำเบื้องต้น Open Water นั้น ผู้เรียนจะลงไปลึกไม่เกิน 12เมตร ในสองไดฟ์ แรก และ ไม่เกิน 18 เมตรในสอง ไดฟ์ต่อมา เมื่อจบคอร์สดำน้ำเบื้องต้นแล้ว คอร์ส AdvancedOpen Water จะพาคุณไป สัมผัสกับระดับที่ลึกขึ้นได้ถึง 40 เมตร แต่โดยปกติที่เราดำน้ำเที่ยวกันเฉลี่ยจะอยู่ที่ประมาณไม่เกิน 18-25 เมตร`
    },
    {
        questionEn: "SHORTSIGHTED DIVERS?",
        questionTh: "สายตาสั้นดำน้ำได้มั้ย",
        content: `สายตาสั้นก็ดำน้ำได้ นักดำน้ำสามารถใส่
                    Contact Lens ได้ หรือ ใส่ MASK ที่เปลี่ยน เลนส์สายตาได้การหักเหของแสงจะทำให้เรา
                    เห็นวัตถุใกล้กว่า 25% และขยายใหญ่กว่า 33% อีกด้วย`
    },
    {
        questionEn: "HOW OLD DIVER?",
        questionTh: "อายุเท่าไหร่ถึงดำน้ำได้",
        content: `สามารถเรียนดำน้ำได้ตั้งแต่ 10 ปีขึ้นไป ถึงอายุ
                    เท่าไหร่ก็ได้ถ้าร่างกายแข็งแรง เริ่มเรียน เมื่ออายุ 8-10 ปี ดำน้ำได้ในสระเท่านั้น เริ่ม
                    เรียนเมื่ออายุ 10 ปีขึ้นไป เรียนดำน้ำได้ปกติ
                    * มีจำกัดความลึกบางช่วงอายุ เริ่มเรียนเมื่อ อายุ 45 ปีขึ้นไป ต้องมีแพทย์เซ็นต์รับรอง Fit for diving
                    แต่เมื่อดำน้ำเป็นแล้ว สามารถ ใช้บัตรดำ น้ำได้ตลอดชีพไม่มีหมดอายุ`
    },
    {
        questionEn: "BUDDY?",
        questionTh: "เรียนดำน้ำคนเดียวได้มั้ย",
        content: `เรียนดำน้ำคนเดียวได้ แต่เราไม่ดำน้ำคน
                    เดียวแน่ ดังนั้นไม่ต้องกังวล มีนักดำน้ำนวน มากที่มาเรียนคนเดียว แล้วมีเพื่อนใหม่จาก
                    การดำน้ำ เป็นแกงค์ใหม่เลยทีเดียว บางคนก็ พบรักจากการดำน้ำด้วยนะ`
    }
]);
</script>

<template>
    <div class="w-full mx-auto py-12 px-4 text-center">
        <h2 class="text-3xl font-bold">Q&A</h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 mt-8 text-left">
            <div v-for="(item, index) in qnaList" :key="index"
                class="flex flex-col justify-start items-center p-6">
                <h3 class="text-xl font-semibold text-center pb-3">{{ item.questionEn }}</h3>
                <div class="w-[33px] mx-auto border-2 border-b border-[#F9E564]"></div>
                <p class="text-black font-medium mt-1 text-center py-3">{{ item.questionTh }}</p>
                <p class="mt-2 text-gray-600">
                    {{ item.content }}
                </p>
            </div>
        </div>
    </div>

</template>



<style scoped></style>