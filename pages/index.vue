<template>
  <article>
    <div class="image">
      <a class="image__text">Najlepsze meble w twojej okolicy</a>
    </div>
    <div class="furniture">
      <FurnitureTile> 
        <svg width="60px" height="60px" viewBox="0 0 24 24" stroke-width="1.5" fill="none" xmlns="http://www.w3.org/2000/svg" color="#ffffff"><path d="M4 18v3M5 10V5a2 2 0 012-2h10a2 2 0 012 2v5" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path><path d="M19.5 10a2.5 2.5 0 00-2.5 2.5V14H7v-1.5a2.5 2.5 0 10-3 2.45V18h16v-3.05a2.5 2.5 0 00-.5-4.95zM20 18v3" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path></svg>
        Krzesła
      </FurnitureTile> 
      <FurnitureTile> 
        <svg width="60px" height="60px" viewBox="0 0 24 24" stroke-width="1.5" fill="none" xmlns="http://www.w3.org/2000/svg" color="#ffffff"><path d="M2 16v3M4 9V7a2 2 0 012-2h12a2 2 0 012 2v2" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path><path d="M20 9a2 2 0 00-2 2v2H6v-2a2 2 0 10-4 0v6h20v-6a2 2 0 00-2-2zM22 16v3" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path></svg>
        Sofy
      </FurnitureTile> 
      <FurnitureTile> 
        <svg width="60px" height="60px" viewBox="0 0 24 24" stroke-width="1.5" fill="none" xmlns="http://www.w3.org/2000/svg" color="#ffffff"><path d="M4 7v10M1 7h22M4 10h16M20 7v10" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path></svg>
        Stoły
      </FurnitureTile> 
      <FurnitureTile> 
        <svg width="60px" height="60px" viewBox="0 0 24 24" stroke-width="1.5" fill="none" xmlns="http://www.w3.org/2000/svg" color="#ffffff"><path d="M6.872 3.428l-2.64 8.8a.6.6 0 00.574.772h14.388a.6.6 0 00.574-.772l-2.64-8.8A.6.6 0 0016.554 3H7.446a.6.6 0 00-.574.428zM12 17v-2M8.6 21h6.8c.331 0 .595-.268.542-.596C15.763 19.29 15.026 17 12 17c-3.026 0-3.763 2.29-3.942 3.404-.053.328.21.596.542.596z" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path></svg>
        Lampy
      </FurnitureTile> 
    </div>
  </article>
</template>

<style lang="scss">
.image{
    background-image: url("~/assets/img/meble.webp");
    height: 700px;
    width: 100%;
    margin: auto;
    background-repeat: no-repeat;
    background-size: 100%;
    box-shadow: inset 0 -250px 250px #121212;
    position: relative;

  &__text{
    font-size: 80px;
    position: absolute;
    bottom: 20px;
    left: 10px;
    color: #fff;
  }
}
.furniture{
    width: 80%;
    margin:10px 10%;
    height: auto;
    display: flex;
    flex-wrap: wrap;
}
</style>
