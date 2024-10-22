<template>
    <div id="products">
      <Product v-for="product in products" :key="product.id" :product="product" />
    </div>
  </template>
  
  <script>
  import Product from './Product.vue'
  
  export default {
    name: 'ProductList',
    components: {
      Product,
    },
    data() {
      return {
        products: [
          {
            id: 1,
            title: 'Lorem Ipsum',
            description: 'Lorem ipsum dolor sit amet consectetur.',
            price: 'R$80,00',
            image: '@/assets/bacarra.png',
          },
          {
            id: 2,
            title: 'Lorem Ipsum',
            description: 'Lorem ipsum dolor sit amet consectetur.',
            price: 'R$80,00',
            image: '@/assets/bacarra.png',
          },
          {
            id: 3,
            title: 'Lorem Ipsum',
            description: 'Lorem ipsum dolor sit amet consectetur.',
            price: 'R$80,00',
            image: '@/assets/bacarra.png',
          },
        ],
      }
    },
  }
  </script>
  
  <style scoped>
  @import '../assets/products.css';
  </style>
  