<script setup>
import { RouterLink } from 'vue-router';
import Footer from '../components/Footer.vue';
</script>


<template>
    <div id="home">
        <div class="container">
            <div class="text">
                <h1>Eyob Abebe Melese</h1>
                <h3>I'm a Fullstack JavaScript developer</h3>
            </div>
            <div class="btns">
                <RouterLink class="about-btn" to="/about">About me</RouterLink>
                <a class="download-btn" download="resume" href="https://eyob-portfolio.netlify.app/images/Resume-Eyob-Melese.pdf">Download resume</a>
            </div>
        </div>
    </div>
    <Footer />
</template>

<style scoped>
@import '../assets/styles/home.css'
</style>
