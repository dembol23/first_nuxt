<template>
    <div class="products">
        <slot></slot>
    </div>
</template>

<style lang="scss" scoped>
  .products{
    width: 90%;
    margin:50px auto;
    display: grid;
    align-items: center;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  }
</style>