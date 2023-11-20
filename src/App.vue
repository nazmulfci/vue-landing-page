<script setup>
import Footer from "./components/Footer.vue";
import Navbar from "./components/Navbar.vue";
import Slider from "./components/Slider.vue";
import About from "./components/About.vue";
</script>

<template>
  <main class="flex-shrink-0">
    <Navbar></Navbar>
    <!-- Header-->
    <!-- <Slider></Slider> -->
    <!-- About Section-->
    <!-- <About></About> -->
    <RouterView />
  </main>
  <Footer></Footer>
</template>

<style scoped></style>
