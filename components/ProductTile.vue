<template>
    <div class="product-tile" >
        <div class="product-tile__img-wrap"><img :src="img" :alt="title" class="product-tile__img"></div>
        <div class="product-tile__name-wrap"><nuxt-link :to="productLink" class="product-tile__name">{{ title }}</nuxt-link></div>
        <div class="product-tile__description-wrap"><p class="product-tile__description">{{ description }}</p></div>
        <p class="product-tile__price">{{ price }} zl,-</p>
    </div>
</template>

<style lang="scss" scoped>
    .product-tile{
    height: min-content;
    border-radius: 15px;
    box-shadow: 0px -10px 53px -13px #BFBFBF;
    padding: 5px;
    margin: 15px;
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;

    &__img-wrap{
        width: 250px;
        height: 250px;
        border-radius: 15px;
        display: flex;
        justify-content: center;
        align-items: center;
    } 
    &__img{
        max-width: 100%;
        max-height: 100%;
        border-radius: 15px;
    }   
    &__name-wrap{
        height: 80px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    &__name{
        text-decoration: none;
        color: #000;
        font-size: 2rem;
        margin-left: 5px;
        text-align: center;
        display: -webkit-box;
        -webkit-line-clamp: 3;
        -webkit-box-orient: vertical;
        overflow: hidden;
    }
    &__name:hover{
        text-decoration: 3px underline #8ECAE6;
    }
    &__description-wrap{
        height: 80px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    &__description{
        color: #000;
        font-size: 1.4rem;
        width: 95%;
        display: -webkit-box;
        -webkit-line-clamp: 3;
        -webkit-box-orient: vertical;
        overflow: hidden;
    }
    &__price{
        color: #000;
        font-size: 2.5rem;
        width: 100%;
        text-align: right;
        margin-right: 25px;
    }
    }
</style>

<script>
    export default{
        props: {
            id: {
                type: Number,
                required: true
            },
            title: {
                type: String,
                required: true
            },
            description: {
                type: String,
                required: true
            },
            price: {
                type: String,
                required: true
            },
            img: {
                type: String,
                required: true
            }
        },
        computed: {
            productLink(){
                return "/produkty/" + this.id
            }
        }
    }
</script>
