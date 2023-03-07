<template>
  <div>
  <div>
    <p>Produkty</p>
  </div>
  <div id="products">
    <!-- <ul>
      <li><nuxt-link to="/produkty/krzeslo">krzesło</nuxt-link></li>
      <li><nuxt-link to="/produkty/stol">stół</nuxt-link></li>
      <li><nuxt-link to="/produkty/lampa">lampa</nuxt-link></li>
    </ul> -->
    <nuxt-link to="/produkty/"><div class="products-tile">
      <img src="~/assets/img/produkty/krzeslo.webp" alt="krzeslo">
      <p style="text-align: center;">Krzesło</p>
      <p style="text-align: right;">190 xl,-</p>
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