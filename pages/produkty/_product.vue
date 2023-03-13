<template>
      <div class="product">
        <div class="product__image">
          <img :src="product.image" :alt="product.title">
        </div>
        <div class="product__info">
          <h2 class="product__info__title">{{ product.title }}</h2>
          <h4 class="product__info__description">{{ product.description }}</h4>
          <h4 class="product__info__price">{{ product.price }} zł</h4>
        </div>
      </div>
</template>

<script>
  import axios from 'axios';
  export default{
    async asyncData({params,error}){
      const productId=params.product
      const api = 'https://fakestoreapi.com/products/' + productId
      let product = []
      try{
        const res = await axios.get(api)
        product = res.data
        product.price = product.price.toFixed(2)
      }
      catch(err){
        console.warn(err)
        error(err)
      }
      return { product }
    }
  }
</script>

<style lang="scss" scoped>
  .product{
    width: 80%;
    margin: 20px auto;
    display: flex;
    &__image{
      width: 55%;
      margin-right: 5%;
      img{
        width: 100%;
      }
    }
    &__info{
      width: 40%;
      display: flex;
      flex-direction: column;
      &__title{
        text-align: center;
        font-size: 3.4rem;
      }
      &__description{
        font-size: 1.9rem;
        color: #121212;
      }
      &__price{
        font-size:6rem;
        text-align: right;
        color: #121212;
      }
    }
  }
</style>