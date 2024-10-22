<template>
    <header>
      <nav id="navbar">
        <i class="fa-solid fa-tents" id="nav_logo">ABC camping</i>
        <ul id="nav_list">
          <li class="nav-item active">
            <a href="#home">INICIO</a>
          </li>
          <li class="nav-item">
            <a href="#catalago">PRODUTOS</a>
          </li>
          <li class="nav-item">
            <a href="#contato">CONTATO</a>
          </li>
        </ul>
        <button class="btn-default">RESERVE AGORA!</button>
        <button id="mobile_btn">
          <i class="fa-solid fa-bars"></i>
        </button>
      </nav>
  
      <div id="mobile_menu">
        <ul id="mobile_nav_list">
          <li class="nav-item">
            <a href="#home">INICIO</a>
          </li>
          <li class="nav-item">
            <a href="#catalago">PRODUTOS</a>
          </li>
          <li class="nav-item">
            <a href="#contato">CONTATO</a>
          </li>
        </ul>
        <button class="btn-default">RESERVE AGORA!</button>
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: 'Header',
  }
  </script>
  
  <style scoped>
  @import '../assets/header.css';
  </style>
  