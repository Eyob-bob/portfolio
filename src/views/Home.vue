<script setup>
import { RouterLink } from 'vue-router';


const date = new Date();

</script>


<template>
    <div id="home">
        <div class="container">
            <div class="text">
                <h1>Eyob Abebe Melese</h1>
                <h3>I'm a Fullstack JavaScript developer</h3>
            </div>
            <RouterLink class="about-btn" to="/about">About me</RouterLink>
        </div>
        <div class="footer">
            <p>© Copyright Eyob {{ date.getFullYear() }}. All Rights Reserved</p>
        </div>
    </div>
</template>

<style scoped>
@import '../assets/styles/home.css'
</style>
