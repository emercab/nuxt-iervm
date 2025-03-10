<script setup>
  useHead({
    titleTemplate: (title) =>
      title
        ? `${title} - Institución Educativa Rafael Valle Meza`
        : 'Institución Educativa Rafael Valle Meza',
  });
</script>

<template>
  <AppTopbar />

  <AppHeader>
    <AppNavbar />
    
    <HeroImage />
  </AppHeader>

  <slot />

  <AppFooter />
</template>
