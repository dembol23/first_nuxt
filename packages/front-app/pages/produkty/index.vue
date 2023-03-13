<template>
  <article>
  <div class="products">
    <ProductTile id=1 name="Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops" price=109.95 img="https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg"></ProductTile>
  </div>
  </article>
</template>
<style lang="scss">
.products{
  width: 80%;
  margin:50px auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
    &__tile{
      width: 250px;
      border-radius: 15px;
      margin: 10px 20px;
      box-shadow: 0px -10px 53px -13px #BFBFBF;
      text-decoration: none;
      padding: 5px;
      &:hover &__name{
      text-decoration: underline;
      }
      &__img{
        width: 100%;
        border-radius: 15px;
      }
      &__name{
        color: #000;
        font-size: 1em;
        margin-left: 5px;
      }
      &__price{
        color: #000;
        font-size: 1.2em;
        text-align: right;
        margin-right: 5px;
      }
    }

}
</style>