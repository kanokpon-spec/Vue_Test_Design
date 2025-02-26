<script setup>
</script>

<template>
    <header class="bg-yellow-400 py-3 px-6 flex items-center justify-between">
        <div class="container mx-auto px-10 flex items-center justify-between">
            <!-- Logo -->
            <div class="flex items-center">
                <img src="/logo.svg" alt="Dive Potato Logo" class="w-12" />
            </div>

            <!-- Navigation -->
            <nav class="hidden md:flex space-x-6 text-black font-base">
                <a href="#" class="hover:text-gray-700">HOME</a>
                <a href="#" class="hover:text-gray-700">ABOUT US</a>
                <a href="#" class="hover:text-gray-700">COURSE</a>
                <a href="#" class="hover:text-gray-700">TRIP</a>
                <a href="#" class="hover:text-gray-700">KNOWLEDGE & BLOG</a>
                <a href="#" class="hover:text-gray-700">EQUIPMENT</a>
                <a href="#" class="hover:text-gray-700">CONTACT US</a>
            </nav>

            <!-- Right Section -->
            <div class="flex items-center space-x-4">
                <!-- Search Icon -->
                <button class="text-black hover:text-gray-700">
                    <img src="/search.svg" alt="">
                </button>

                <!-- Login / Create Account -->
                <div class="text-black">
                    <a href="#" class="hover:text-gray-700">login</a>
                    <span class="mx-1">|</span>
                    <a href="#" class="hover:text-gray-700">Create Account</a>
                </div>

                <!-- Shopping Cart -->
                <button class="text-black hover:text-gray-700">
                    <img src="/cart.svg" alt="">
                </button>

                <!-- Language Switch -->
                <div class="text-black">
                    <a href="#" class="text-[#BE901B]">ENG</a>
                    <span class="mx-1">|</span>
                    <a href="#" class="hover:text-gray-700">THA</a>
                </div>
            </div>
        </div>
    </header>
</template>