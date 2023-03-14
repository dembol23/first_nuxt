<template>
    <div class="product">
        <slot></slot>
    </div>
</template>

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