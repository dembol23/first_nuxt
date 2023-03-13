<template>
    <nav class="nav">
        <div class="nav__title-wrap"><h1 class="nav__title">Sklep</h1></div>
        <nuxt-link to="/" class="nav__link">Strona główna</nuxt-link>
        <nuxt-link to="/produkty" class="nav__link">Produkty</nuxt-link>
        <hr>
    </nav>  
</template>
<style lang="scss">
    .nav{
        background-color: #8ecae6;
        display: flex;
        align-items: center;
        color: #fff;
        &__title{
            font-size: 50px;
            padding: 0;
            margin: 0 30px;
        }
        &__link{
            padding: 40px;
            color: #fff;
            text-transform: uppercase;
            font-size: 20px;
            text-decoration: none;
        }
        &__link:hover{
            background-color: #AED9ED;
        }
    }
    @media(max-width:920px){
        .nav{
            flex-direction: column;
            justify-content: center;
            &__title{
                text-align: center;
                padding: 10px 0;
            }
            &__link{
                width: 100%;
                text-align: center;
            }
        }
    } 
</style>
