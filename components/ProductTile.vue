<template>
    <nuxt-link :to="productLink" class="products__tile">
      <img :src="img" :alt="name" class="products__tile__img">
      <p class="products__tile__name">{{ name }}</p>
      <p class="products__tile__price">{{ price }} zl,-</p>
    </nuxt-link>
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
</style>
<script>
    export default{
        props: {
            id: {
                type: Number,
                required: true
            },
            name: {
                type: String,
                required: true
            },
            price: {
                type: Number,
                required: true
            },
            img: {
                type: String,
                required: true
            }

        },
        computed: {
            productLink:{
                get(){
                    return "/produkty/" + this.id
                }
            }
        }
    }
</script>
