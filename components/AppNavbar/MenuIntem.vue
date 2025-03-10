<script setup lang="ts">
  const { title, url } = defineProps<{
    title: string;
    url: string;
  }>();
</script>

<template>
  <NuxtLink
    :to="url"
    class="hover:text-blue-600"
  >
    {{ title }}
  </NuxtLink>
</template>

<style scoped></style>
