<script setup>
import Footer from '../components/Footer.vue';

</script>

<template>

    <div class="about-me-page">

        <div id="about">
            <h2 class="title">About</h2>
            <div class="about-me">
                <img src="/images/background.jpg" alt="My Image">
                <div class="info">
                    <h3>Fullstack JavaScript and Mobile App Developer</h3>
                    <p>My Personal Informations</p>
                    <div class="personal-info">
                        <p><span>Birthday:</span> 15 Nov 2000</p>
                        <p><span>Email:</span> eabebe91@gmail.com</p>
                        <p><span>Phone:</span> +251 964643164</p>
                        <p><span>City:</span> Gondar, Amhara, Ethiopia</p>
                        <p><span>Age:</span> 21</p>
                    </div>
                </div>
            </div>
        </div>

        <div id="skills">
            <h2 class="title">Skills</h2>

            <div class="skills">

                <div class="skill-container">
                    <p>React</p>
                    <div class="skill">
                        <div class="progress x-90">90%</div>
                    </div>
                </div>
                <div class="skill-container">
                    <p>Vue js</p>
                    <div class="skill">
                        <div class="progress x-90">90%</div>
                    </div>
                </div>
                <div class="skill-container">
                    <p>Node js</p>
                    <div class="skill">
                        <div class="progress x-80">80%</div>
                    </div>
                </div>
                <div class="skill-container">
                    <p>Express js</p>
                    <div class="skill">
                        <div class="progress x-80">80%</div>
                    </div>
                </div>
                <div class="skill-container">
                    <p>GraphQL</p>
                    <div class="skill">
                        <div class="progress x-60">60%</div>
                    </div>
                </div>
                <div class="skill-container">
                    <p>Postgress SQL</p>
                    <div class="skill">
                        <div class="progress x-60">60%</div>
                    </div>
                </div>
            </div>
        </div>

        <Footer />
    </div>

</template>

<style scoped>
@import '../assets/styles/about.css'
</style>