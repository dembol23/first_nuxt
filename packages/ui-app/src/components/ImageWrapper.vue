<template>
    <div class="image">
      <a class="image__text">Najlepsze meble w twojej okolicy</a>
    </div>
</template>

<style lang="scss" scoped>
.image{
    background-image: url("~/assets/img/meble.webp");
    height: 800px;
    width: 100%;
    background-repeat: no-repeat;
    background-size: 100vw;
    box-shadow: inset 0 -250px 250px #121212;
    position: relative;

  &__text{
    font-size: 8rem;
    position: absolute;
    bottom: 20px;
    left: 10px;
    color: #FFF;
  }
}
</style>