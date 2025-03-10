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

  <AppNavbar />

  <slot />

  <AppFooter />
</template>
