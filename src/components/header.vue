<template>
  <header class="w-full py-7 px-[8%]">
    <nav id="navbar" class="w-full flex items-center justify-between">
      <i class="fa-solid fa-tents text-2xl text-gray-800" id="nav_logo">ABC camping</i>
      <ul id="nav_list" class="hidden md:flex list-none gap-12">
        <li :class="{ 'font-bold text-blue-500 border-b-3 border-gray-800': activeSection === 'home' }" class="nav-item">
          <a href="#home" @click="setActiveSection('home')" class="text-gray-800 font-semibold hover:text-blue-600">INICIO</a>
        </li>
        <li :class="{ 'font-bold text-blue-500 border-b-3 border-gray-800': activeSection === 'produto' }" class="nav-item">
          <a href="#produto" @click="setActiveSection('produto')" class="text-gray-800 font-semibold hover:text-blue-600">PRODUTOS</a>
        </li>
        <li :class="{ 'font-bold text-blue-500 border-b-3 border-gray-800': activeSection === 'contato' }" class="nav-item">
          <a href="#contato" @click="setActiveSection('contato')" class="text-gray-800 font-semibold hover:text-blue-600">CONTATO</a>
        </li>
      </ul>
      <div class="flex items-center space-x-4">
        <button class="hidden md:block bg-yellow-500 text-white py-2 px-4 rounded hover:bg-yellow-600">RESERVE AGORA!</button>
        <button id="mobile_btn" @click="toggleMobileMenu" class="md:hidden text-gray-800 text-2xl bg-transparent cursor-pointer">
          <i class="fa-solid fa-bars"></i>
        </button>
      </div>
    </nav>

    <div id="mobile_menu" v-if="isMobileMenuOpen" class="md:hidden flex flex-col items-center bg-gray-200 p-4">
      <ul id="mobile_nav_list" class="flex flex-col gap-3 my-3">
        <li class="nav-item">
          <a href="#home" @click="setActiveSection('home'); toggleMobileMenu()" class="text-gray-800 font-semibold hover:text-blue-600">INICIO</a>
        </li>
        <li class="nav-item">
          <a href="#produto" @click="setActiveSection('produto'); toggleMobileMenu()" class="text-gray-800 font-semibold hover:text-blue-600">PRODUTOS</a>
        </li>
        <li class="nav-item">
          <a href="#contato" @click="setActiveSection('contato'); toggleMobileMenu()" class="text-gray-800 font-semibold hover:text-blue-600">CONTATO</a>
        </li>
      </ul>
      <button class="bg-yellow-500 text-white py-2 px-4 mt-4 rounded hover:bg-yellow-600">RESERVE AGORA!</button>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isMobileMenuOpen: false,
      activeSection: 'home',
    };
  },
  methods: {
    toggleMobileMenu() {
      this.isMobileMenuOpen = !this.isMobileMenuOpen;
    },
    setActiveSection(section) {
      this.activeSection = section;
    },
  },
};
</script>
