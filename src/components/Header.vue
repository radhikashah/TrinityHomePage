<script setup>
    import Navigation from './Navigation.vue';
    import IconLogin from './icons/IconLogin.vue';
</script>

<template>
    <div class="flex flex-end md:grid md:grid-cols-2">
        <div class="header-logo flex">
            <img src="./../assets/TrinityLogo.png" alt="" />
            <img src="./../assets/img-celebration-50.png" alt="" />
        </div>

        <a class="login xl:hidden flex items-center flex-end" href="/login" aria-label="Login">
            <IconLogin />
        </a>

        <Navigation />
    </div>
</template>