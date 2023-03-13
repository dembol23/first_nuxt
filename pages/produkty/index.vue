<template>
    <div class="products">
      <ProductTile v-for="value in productsList" :key="value['id']" :id="value['id']" :title="value['title']" :description="value['description']" :price="value['price'].toFixed(2)" :img="value['image']"></ProductTile>
    </div>
</template>
<style lang="scss">
.products{
  width: 90%;
  margin:50px auto;
  display: grid;
  align-items: center;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
}
</style>
<script>
  import axios from 'axios';
  export default{
    async asyncData(){
      const api = 'https://fakestoreapi.com/products'
      const res = await axios.get(api)
      const productsList = res.data
      return { productsList }
    }
  }
</script>