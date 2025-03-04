<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);
</script>

<template>
    <header class="bg-yellow-400 py-3 px-6">
        <div class="container mx-auto px-0 md:px-4 flex items-center justify-between">
            <!-- Logo -->
            <div class="flex items-center">
                <img src="/logo.svg" alt="Dive Potato Logo" class="w-8 md:w-12" />
            </div>

            <!-- Mobile Menu Button -->
            <button @click="isMenuOpen = !isMenuOpen" class="xl:hidden  text-black focus:outline-none">
                <!-- <img src="/menu.svg" alt="Menu" class="w-6"> -->
                <svg class="w-8 h-8 md:w-10 md:h-10" xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="100" height="100"
                    viewBox="0 0 50 50">
                    <path
                        d="M 0 9 L 0 11 L 50 11 L 50 9 Z M 0 24 L 0 26 L 50 26 L 50 24 Z M 0 39 L 0 41 L 50 41 L 50 39 Z">
                    </path>
                </svg>
            </button>

            <!-- Navigation for Desktop -->
            <nav class="hidden xl:flex space-x-5 text-black font-base">
                <a href="#" class="hover:text-gray-700">HOME</a>
                <a href="#" class="hover:text-gray-700">ABOUT US</a>
                <a href="#" class="hover:text-gray-700">COURSE</a>
                <a href="#" class="hover:text-gray-700">TRIP</a>
                <a href="#" class="hover:text-gray-700">KNOWLEDGE & BLOG</a>
                <a href="#" class="hover:text-gray-700">EQUIPMENT</a>
                <a href="#" class="hover:text-gray-700">CONTACT US</a>
            </nav>

            <!-- Mobile Menu (Slide In) -->
            <div class="fixed top-0 z-10 right-0 w-64 h-full bg-yellow-400 shadow-lg transform transition-transform duration-300 ease-in-out"
                :class="isMenuOpen ? 'translate-y-0' : 'translate-x-full'">
                <button @click="isMenuOpen = false" class="absolute top-4 right-4 text-black text-xl">
                    ✕
                </button>
                <nav class="flex flex-col mt-10 space-y-4 text-black font-base p-6">
                    <a href="#" class="hover:text-gray-700">HOME</a>
                    <a href="#" class="hover:text-gray-700">ABOUT US</a>
                    <a href="#" class="hover:text-gray-700">COURSE</a>
                    <a href="#" class="hover:text-gray-700">TRIP</a>
                    <a href="#" class="hover:text-gray-700">KNOWLEDGE & BLOG</a>
                    <a href="#" class="hover:text-gray-700">EQUIPMENT</a>
                    <a href="#" class="hover:text-gray-700">CONTACT US</a>
                </nav>
            </div>

            <!-- Right Section -->
            <div class="hidden xl:flex  items-center space-x-5">
                <button class="text-black hover:text-gray-700">
                    <img src="/search.svg" alt="Search">
                </button>
                <div class="text-black">
                    <a href="#" class="hover:text-gray-700">Login</a>
                    <span class="mx-1">|</span>
                    <a href="#" class="hover:text-gray-700">Create Account</a>
                </div>
                <button class="text-black hover:text-gray-700">
                    <img src="/cart.svg" alt="Cart">
                </button>
                <div class="text-black">
                    <a href="#" class="text-[#BE901B]">ENG</a>
                    <span class="mx-1">|</span>
                    <a href="#" class="hover:text-gray-700">THA</a>
                </div>
            </div>
        </div>
    </header>
</template>
