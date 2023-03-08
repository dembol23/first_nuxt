<template>
    <nav class="nav">
        <div class="nav__title">Meble</div>
        <nuxt-link to="/" class="nav__link">Strona główna</nuxt-link>
        <nuxt-link to="/produkty" class="nav__link">Produkty</nuxt-link>
        <hr>
    </nav>  
</template>
<style scoped>
.nav{
    background-color: #8ecae6;
    display: flex;
    align-items: center;
    color: #fff;
}
.nav__title{
    font-size: 50px;
    padding: 0;
    margin: 0 30px;
}
.nav__link{
    padding: 40px;
    color: #fff;
    text-transform: uppercase;
    font-size: 20px;
    text-decoration: none;
}
.nav__link:hover{
    background-color: #AED9ED;
}
</style>
