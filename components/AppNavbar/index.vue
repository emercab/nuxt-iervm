<script setup lang="ts"></script>

<template>
  <!-- Navbar -->
  <nav
    class="top-0 w-full bg-white bg-opacity-30 backdrop-blur-lg shadow-md z-50"
  >
    <div class="container mx-auto flex justify-between items-center px-4 py-3">
      <a href="#" class="text-xl font-bold text-gray-800">Universidad</a>

      <!-- Menú en pantallas grandes -->
      <div class="hidden md:flex space-x-6">
        <a href="#" class="hover:text-blue-600">Inicio</a>
        <a href="#" class="hover:text-blue-600">Nosotros</a>
        <a href="#" class="hover:text-blue-600">Carreras</a>
        <a href="#" class="hover:text-blue-600">Contacto</a>
      </div>

      <!-- Botón del menú en móvil -->
      <button id="menu-toggle" class="md:hidden text-gray-800">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="size-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M3.75 5.25h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5"
          />
        </svg>
      </button>
    </div>

    <!-- Menú en pantallas pequeñas -->
    <div id="mobile-menu" class="hidden md:hidden bg-white bg-opacity-90">
      <a href="#" class="block py-2 px-4">Inicio</a>
      <a href="#" class="block py-2 px-4">Nosotros</a>
      <a href="#" class="block py-2 px-4">Carreras</a>
      <a href="#" class="block py-2 px-4">Contacto</a>
    </div>
  </nav>
</template>

<style scoped></style>
