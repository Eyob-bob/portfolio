<script setup>
const date = new Date();

</script>

<template>
    <div class="footer">
        <p>© Copyright Eyob {{ date.getFullYear() }}. All Rights Reserved</p>
    </div>
</template>

<style scoped>
.footer {
    background-color: #e9e8e6;
    height: 3rem;
    display: grid;
    place-content: center;
}

.footer p {
    font-weight: 600;
}

@media (max-width: 370px) {
    .footer p {
        font-size: .7rem;
    }
}
</style>