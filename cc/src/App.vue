<script>
import GalleryItem from './components/GalleryItem.vue';

import CreditCardCheckout from './components/CreditCardCheckout.vue';
import LoginForm from './components/LoginForm.vue'

export default {
  name: 'App',
  components: { GalleryItem, LoginForm, CreditCardCheckout },
  data() {
    return {
        LoginForm: 'LoginForm',
        CreditCardCheckout: 'CreditCardCheckout'
    };
  }
};
</script>

<template>
    <div class="app-wrapper flex flex-col gap-5 items-center">
        <h1 class="text-4xl mt-4">Daily UI components gallery</h1>
        <img class="w-32" src="/uiDesignDaily.png" alt="UI Design Daily changed logo">
        <GalleryItem
            title="Sign Up"
            date="10 Mar 2016"
            dailyUILink="https://uidesigndaily.com/posts/photoshop-sign-up-authentication-day-1">
            <component :is="LoginForm"></component>
        </GalleryItem>

        <GalleryItem
            title="Lorem"
            date="10 Mar 2016"
            dailyUILink="https://example.com">
            <component :is="CreditCardCheckout"></component>
        </GalleryItem>
    
    </div>
</template>
