<template>
  <div>
  <div id="products">
    <!-- <ul>
      <li><nuxt-link to="/produkty/krzeslo">krzesło</nuxt-link></li>
      <li><nuxt-link to="/produkty/stol">stół</nuxt-link></li>
      <li><nuxt-link to="/produkty/lampa">lampa</nuxt-link></li>
    </ul> -->
    <nuxt-link to="/produkty/krzeslo" style="text-decoration: none;"><div class="products-tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo">
      <p style="text-align: left;">Krzesło</p>
      <p style="text-align: right;">190 zl,-</p>
    </div></nuxt-link>
    <nuxt-link to="/produkty/krzeslo" style="text-decoration: none;"><div class="products-tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo">
      <p style="text-align: left;">Krzesło</p>
      <p style="text-align: right;">190 zl,-</p>
    </div></nuxt-link>
    <nuxt-link to="/produkty/krzeslo" style="text-decoration: none;"><div class="products-tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo">
      <p style="text-align: left;">Krzesło</p>
      <p style="text-align: right;">190 zl,-</p>
    </div></nuxt-link>
    <nuxt-link to="/produkty/krzeslo" style="text-decoration: none;"><div class="products-tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo">
      <p style="text-align: left;">Krzesło</p>
      <p style="text-align: right;">190 zl,-</p>
    </div></nuxt-link>
    <nuxt-link to="/produkty/krzeslo" style="text-decoration: none;"><div class="products-tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo">
      <p style="text-align: left;">Krzesło</p>
      <p style="text-align: right;">190 zl,-</p>
    </div></nuxt-link>
  </div>
</div>
</template>
<script>
export default{
    layout:'strona',
    created(){
      console.log(process.server)
    }
}
</script>