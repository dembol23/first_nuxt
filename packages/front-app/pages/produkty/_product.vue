<template>
  <ProductPage>
    <div class="product__image">
      <img :src="product.image" :alt="product.title">
    </div>
    <div class="product__info">
      <h2 class="product__info__title">{{ product.title }}</h2>
      <h4 class="product__info__description">{{ product.description }}</h4>
      <h4 class="product__info__price">{{ product.price }} zł</h4>
    </div>
  </ProductPage>
</template>

<script>
  import ProductPage from 'ui-app/src/components/ProductPage.vue';
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
    },
    components:{
      ProductPage
    }
  }
</script>