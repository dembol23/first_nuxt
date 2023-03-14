<template>
    <ProductsList>
      <ProductTile v-for="value in productsList" :key="value.id" :id="value.id" :title="value.title" :description="value.description" :price="value.price.toFixed(2)" :img="value.image"></ProductTile>
    </ProductsList>
</template>

<script>
  import ProductTile from 'ui-app/src/components/ProductTile.vue';
  import ProductsList from 'ui-app/src/components/ProductsList.vue';
  import axios from 'axios';
  export default{
    async asyncData(error){
      const api = 'https://fakestoreapi.com/products'
      let productsList = []
      try{
        const res = await axios.get(api)
        productsList = res.data
      }
      catch(err){
        console.warn(err)
        error(err)
      }
      return { productsList }
    },
    components:{
      ProductTile,
      ProductsList
    }
  }
</script>