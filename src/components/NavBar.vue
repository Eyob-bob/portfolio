<script setup>
import { ref, watchEffect } from 'vue';
import { RouterLink } from 'vue-router';

const navLinks = ref('element')
const hamberger = ref('element')
const navLink = ref('element')

function toggleSidebar() {
    if (navLinks.value.dataset.visibility === 'false') {
        navLinks.value.dataset.visibility = 'true'
        hamberger.value.setAttribute('aria-expanded', true)
    }

    else {
        navLinks.value.dataset.visibility = 'false'
        hamberger.value.setAttribute('aria-expanded', false)
    }
}

function navLinkClicked() {
    navLinks.value.dataset.visibility = 'false'
    hamberger.value.setAttribute('aria-expanded', false)
}
</script>


<template>
    <nav>
        <RouterLink class="logo-text" to="/">Eyob <span>.</span></RouterLink>

        <ul ref="navLinks" class="nav-links" data-visibility="false">
            <li @click="navLinkClicked" class="nav-link">
                <RouterLink class="link" to="/">Home</RouterLink>
            </li>
            <li @click="navLinkClicked" class="nav-link">
                <RouterLink class="link" to="/about">About</RouterLink>
            </li>
            <li @click="navLinkClicked" class="nav-link">
                <RouterLink class="link" to="/projects">Projects</RouterLink>
            </li>
        </ul>

        <div ref="hamberger" aria-expanded="false" @click="toggleSidebar" class="hamberger">
            <div></div>
            <div></div>
            <div></div>
        </div>
    </nav>
</template>

<style scoped>
@import '../assets/nav-bar.css';
</style>