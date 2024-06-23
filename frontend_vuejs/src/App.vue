<script setup lang="ts">
    import { RouterLink, RouterView } from "vue-router";
    import Profile from './components/mainpage/Profile.vue'
    import About from './components/mainpage/About.vue'
    import Studies from './components/mainpage/Studies.vue'
    import Contact from './components/mainpage/Contact.vue'
    import Navbar from './components/Navbar.vue'
</script>

<template>
    <Navbar/>
    <Profile class="mt-12"/>
    <div class="bodyMargin">
        <About/>
        <Studies/>
        <Contact/>
    </div>
</template>

<style scoped>
    .bodyMargin {
        margin-top: 3.5rem;
        margin-left: 5%;
        margin-right: 5%;
        margin-bottom: 10rem;
    }
    @media (min-width: 640px) {
        .bodyMargin {
            margin-left: 10%;
            margin-right: 10%;
        }
    }
    @media (min-width: 768px) {
        .bodyMargin {
            margin-left: 15%;
            margin-right: 15%;
        }
    }
    @media(min-width: 1024px) {
        .bodyMargin {
            margin-left: 20%;
            margin-right: 20%;
        }
    }
    @media(min-width: 1280px) {
        .bodyMargin {
            margin-left: 25%;
            margin-right: 25%;
        }
    }
</style>
