<script setup lang="ts"></script>

<template>
  <!-- Navbar -->
  <nav class="top-0 w-full bg-white/30 backdrop-blur-lg shadow-md z-50">
    <div class="container mx-auto flex justify-between items-center px-4 py-3">
      <!-- Logo -->
      <AppNavbarLogo>Universidad</AppNavbarLogo>

      <!-- Menú en pantallas grandes -->
      <AppNavbarMainMenu />

      <!-- Botón del menú en móvil -->
      <AppNavbarMobileButton />
    </div>

    <!-- Menú en pantallas pequeñas -->
    <AppNavbarMobileMenu />
  </nav>
</template>

<style scoped></style>
