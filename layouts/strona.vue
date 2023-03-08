<template>
    <div id="main">
        <div id="menu">
            <div id="title">Meble</div>
            <nuxt-link to="/" style="text-decoration: none;"><div class="link"><a>Strona główna</a></div></nuxt-link>
            <nuxt-link to="/produkty/" style="text-decoration: none;"><div class="link"><a>Produkty</a></div></nuxt-link>
            <hr>
        </div>
        <div id="content">
            <nuxt/>
        </div>
    </div>
</template>
<script>
export default {}
</script>
<style scoped>
@import '~/assets/css/main.css';
</style> 