<script setup>
import LoginForm from './components/LoginForm.vue'
import CreditCardCheckout from './components/CreditCardCheckout.vue';
</script>

<template>
    <div class="app-wrapper flex flex-col gap-5 items-center">
        <LoginForm/>
        <CreditCardCheckout/>
    </div>
</template>
