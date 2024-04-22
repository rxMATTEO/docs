<script setup lang="ts">
defineProps<{
  imgUrl: string
}>();
</script>

<template>
  <div>
    Это контейнер для изображения {{ imgUrl }}
    <img :src="imgUrl" alt="image">
    <ContentSlot unwrap="button" :use="$slots.description" />
  </div>
</template>
