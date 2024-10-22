<template>
    <div class="product">
      <div class="product-heart">
        <i class="fa-solid fa-heart"></i>
      </div>
  
      <img :src="product.image" class="dish-image" alt="" />
  
      <h3 class="product-title">{{ product.title }}</h3>
  
      <span class="product-description">{{ product.description }}</span>
  
      <div class="product-rate">
        <i class="fa-solid fa-star" v-for="n in 5" :key="n"></i>
        <span>(500+)</span>
      </div>
  
      <div class="product-price">
        <h4>{{ product.price }}</h4>
        <button class="btn-default">
          <i class="fa-solid fa-basket-shopping"></i>
        </button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Product',
    props: {
      product: Object,
    },
  }
  </script>
  
  <style scoped>
  @import '../assets/products.css';
  </style>
  