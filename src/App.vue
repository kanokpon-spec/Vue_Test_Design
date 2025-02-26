<script setup>
import Header from './components/Header/index.vue'
import Footer from './components/Footer/index.vue'
</script>

<template>
  <div class="">
    <Header />
    <main>
      <div>
        <router-view />
      </div>
    </main>
    <Footer />
  </div>
</template>
