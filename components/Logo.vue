<script setup lang="ts">
const { config } = useDocus();
</script>

<template>
  <div class="logo">
    <img src="/img/logo.avif" alt="Plex CRM">
    <ProseH3 class="logo__title">
      {{ config.title }}
    </ProseH3>
  </div>
</template>

<style>
.logo{
  display: flex;
  align-items: center;
  gap: 16px;
}

.logo__title {
  margin: 0 !important;
}
</style>