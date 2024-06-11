<template>
    <nav>
        <div class="nav-logo">
            <img :src="logo" alt="BizKit Logo">
            <i class="pi pi-bars"></i>
        </div>
        <div class="nav-tools">
            <p>tools</p>
        </div>
    </nav>
</template>

<script setup>
import logo from '../assets/img/bzlogo.png';

</script>

<style scoped>
nav {
    height: 3rem;
    display: flex;
    position: fixed;
    width: 100%;
    top: 0;
    justify-content: space-between;
    padding: 12px;
    background-color: var(--color-white);
    color: var(--color-black);
}

.nav-logo{
    display: flex;
    gap: 3rem;
    margin: auto 0;
}

.nav-logo img {
    width: 30%;
    margin: auto 0;
}

</style>