<template>
    <div id="app">
      <Header />
      <main id="content">
        <section id="home">
          <div class="shape"></div>
          <div id="cta">
            <h1 class="title">
              Transforme sua aventura em uma experiência <span>inesquecível</span>
            </h1>
  
            <div id="cta_buttons">
              <a href="#catalago" class="btn-default">VER PRODUTOS</a>
              <a href="tel:+5588999041272" id="phone_button">
                <button class="btn-default">
                  <i class="fa-solid fa-phone"></i>
                </button>
                (88) 99904-1272
              </a>
            </div>
  
            <div class="social-media-buttons">
              <a href="https://tr.ee/-0SSbsYhi7">
                <i class="fa-brands fa-whatsapp"></i>
              </a>
              <a href="https://www.instagram.com/abccamping">
                <i class="fa-brands fa-instagram"></i>
              </a>
              <a href="https://www.tiktok.com/@abccampingce">
                <i class="fa-brands fa-tiktok"></i>
              </a>
            </div>
          </div>
  
          <div id="banner">
            <img src="@/assets/img-home.jpeg" alt="Banner" />
          </div>
        </section>
  
        <section id="catalago">
          <h2 class="section-title">Produtos</h2>
          <ProductList />
        </section>
      </main>
    </div>
  </template>
  
  <script>
  import Header from './components/Header.vue'
  import ProductList from './components/ProductList.vue'
  
  export default {
    name: 'App',
    components: {
      Header,
      ProductList,
    },
  }
  </script>
  
  <style scoped>
  @import './assets/style.css';
  @import './assets/header.css';
  @import './assets/home.css';
  @import './assets/products.css';
  </style>
  