<template>
      <div class="product">
        <div class="product__image">
          <img :src="product['image']" :alt="product['title']">
        </div>
        <div class="product__info">
          <h2 class="product__info__title">{{ product['title'] }}</h2>
          <h4 class="product__info__description">{{ product['description'] }}</h4>
          <h4 class="product__info__price">{{ product['price'] }} zł</h4>
        </div>
      </div>
</template>

<script>
  import axios from 'axios';
  export default{
    async asyncData({params}){
      const productId=params['product']
      const api = 'https://fakestoreapi.com/products/' + productId
      const res = await axios.get(api)
      const product = res.data
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
        font-size: 34px;
      }
      &__description{
        font-size: 19px;
        color: #121212;
      }
      &__price{
        font-size:60px;
        text-align: right;
        color: #121212;
      }
      
    }

  }
</style>