<script setup lang="ts">
defineProps<{
  imgUrl: string
}>();
</script>

<template>
  <div>
    Это контейнер для изображения {{ imgUrl }}
    <ContentSlot unwrap="button" :use="$slots.description" />
  </div>
</template>
