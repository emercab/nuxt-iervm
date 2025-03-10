<script setup lang="ts">
  const isMobileMenuOpen = ref<boolean>(false);

  const toggleMobileMenu = () => {
    isMobileMenuOpen.value = !isMobileMenuOpen.value;
  };
</script>

<template>
  <!-- Navbar -->
  <nav class="relative top-0 w-full bg-white/50 shadow-md z-50">
    <div class="container mx-auto flex justify-between items-center px-4 py-2">
      <!-- Logo -->
      <AppNavbarLogo>IE Rafael Valle Meza</AppNavbarLogo>

      <!-- Menú en pantallas grandes -->
      <AppNavbarMainMenu />

      <!-- Botón del menú en móvil -->
      <AppNavbarMobileButton @click="toggleMobileMenu" />
    </div>

    <!-- Menú en pantallas pequeñas -->
    <Transition name="slide">
      <AppNavbarMobileMenu v-if="isMobileMenuOpen" class="overflow-hidden" />
    </Transition>
  </nav>
</template>

<style scoped>
/* Animación de deslizamiento */
.slide-enter-active,
.slide-leave-active {
  transition: max-height 0.3s ease-in-out, opacity 0.3s ease-in-out, transform 0.3s ease-in-out;
}

.slide-enter-from {
  max-height: 0;
  opacity: 0;
  transform: translateY(-20px);
}

.slide-enter-to {
  max-height: 500px; /* Ajusta según el tamaño de tu menú */
  opacity: 1;
  transform: translateY(0);
}

.slide-leave-from {
  max-height: 500px;
  opacity: 1;
  transform: translateY(0);
}

.slide-leave-to {
  max-height: 0;
  opacity: 0;
  transform: translateY(-20px);
}
</style>