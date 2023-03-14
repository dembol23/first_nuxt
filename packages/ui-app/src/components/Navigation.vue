<template>
    <nav class="nav">
        <div class="nav__title-wrap"><h1 class="nav__title">Sklep</h1></div>
        <nuxt-link to="/" class="nav__link">Strona główna</nuxt-link>
        <nuxt-link to="/produkty" class="nav__link">Produkty</nuxt-link>
        <hr>
    </nav>  
</template>
<style lang="scss" scoped>
    .nav{
        background-color: #8ECAE6;
        display: flex;
        align-items: center;
        color: #fff;
        &__title{
            font-size: 5rem;
            padding: 0;
            margin: 0 30px;
        }
        &__link{
            padding: 4rem;
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
