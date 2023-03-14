<template>
  <ProductPage :product="product"/>
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