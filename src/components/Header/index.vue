<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);
</script>

<template>
    <header class="bg-yellow-400 py-3 px-6">
        <div class="container mx-auto px-4 flex items-center justify-between">
            <!-- Logo -->
            <div class="flex items-center">
                <img src="/logo.svg" alt="Dive Potato Logo" class="w-12" />
            </div>

            <!-- Mobile Menu Button -->
            <button @click="isMenuOpen = !isMenuOpen" class="md:hidden text-black focus:outline-none">
                <img src="" alt="Menu" class="w-6">
            </button>

            <!-- Navigation -->
            <nav :class="{'hidden lg:flex': !isMenuOpen, 'flex flex-col absolute top-23 left-0 w-full bg-yellow-400 xl:relative z-10 md:flex-row md:space-x-6 md:top-0 md:w-auto': isMenuOpen}" class="space-x-5 space-y-2 md:space-y-0 text-black font-base text-center md:text-left">
                <a href="#" class="hover:text-gray-700 block py-2 md:py-0">HOME</a>
                <a href="#" class="hover:text-gray-700 block py-2 md:py-0">ABOUT US</a>
                <a href="#" class="hover:text-gray-700 block py-2 md:py-0">COURSE</a>
                <a href="#" class="hover:text-gray-700 block py-2 md:py-0">TRIP</a>
                <a href="#" class="hover:text-gray-700 block py-2 md:py-0">KNOWLEDGE & BLOG</a>
                <a href="#" class="hover:text-gray-700 block py-2 md:py-0">EQUIPMENT</a>
                <a href="#" class="hover:text-gray-700 block py-2 md:py-0">CONTACT US</a>
            </nav>

            <!-- Right Section -->
            <div class="hidden md:flex items-center space-x-4">
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
