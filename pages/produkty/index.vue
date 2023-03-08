<template>
  <article class="article">
  <div class="products">
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
    <nuxt-link to="/produkty/krzeslo" class="products__tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo" class="products__tile__img">
      <p class="products__tile__name">Krzesło</p>
      <p class="products__tile__price">190 zl,-</p>
    </nuxt-link>
  </div>
  </article>
</template>
<style scoped>
.products{
  width: 80%;
  margin:50px auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
}
.products__tile{
  width: 250px;
  height: 350px;
  border-radius: 15px;
  margin: 10px 20px;
  /* box-shadow: 0px -15px 48px -19px rgba(150, 150, 150, 1); */
  box-shadow: 0px -10px 53px -13px rgba(191, 191, 191, 1);
  text-decoration: none;
}
.products__tile__img{
  width: 100%;
  height: 250px;
  border-radius: 15px;
}
.products__tile__name{
  color: #000;
  font-size: 1em;
  margin-left: 5px;
}
.products__tile__price{
  color: #000;
  font-size: 1.2em;
  text-align: right;
  margin-right: 5px;
}
</style>