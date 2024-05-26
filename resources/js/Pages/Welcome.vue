<script setup>
import { Head, Link } from '@inertiajs/vue3';

defineProps({
    canLogin: {
        type: Boolean,
    },
    canRegister: {
        type: Boolean,
    },
    laravelVersion: {
        type: String,
        required: true,
    },
    phpVersion: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <Head title="Welcome" />
    <div class="home">
        <div class="content">
            <img src="https://cdn2.hubspot.net/hubfs/4001288/ecommerce-subway-studio-malaysia%20%281%29.gif" alt=""  class="center-image" width="500px" >
            <p class="text-center text-4xl font-bold text-white mt-20">Welcome to Shopee!</p>
            <p class="text-center text-xl font-bold text-white mt-2">Discover and shop for your favorite products</p>
            <p class="text-center text-xl font-bold text-blue-600 mt-5 mb-5">Start shopping now!</p>
            <div class="auth-links">
                <div class="auth-links-container">
                    <Link :href="route('login')" class="route-link">Log in</Link>
                    <Link v-if="canRegister" :href="route('register')" class="route-link">Register</Link>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.home {
    background-image: url('https://img.freepik.com/free-photo/shopping-bag-cart_23-2148879372.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.content {
    text-align: center;
}

.auth-links {
    position: absolute;
    top: 60%;
    right: 830px;
    transform: translateY(-50%);
}

.auth-links-container {
    display: flex;
    align-items: center;
}

.route-link {
    font-weight: 600;
    margin: 10px;
    padding: 8px 16px;
    border: 2px solid transparent;
    border-radius: 4px;
    transition: all 0.3s ease;
    background-color: #4a90e2;
    color: #fff;
    text-decoration: none;
    box-shadow: 0 5px 6px rgba(0, 0, 0, 0.1);
}

.route-link:hover {
    background-color: #fff;
    border-color: #4a90e2;
    color: #4a90e2;
}
</style>
