<script setup lang="ts">
defineProps<{
  imgUrl: string
}>();
</script>

<template>
  <div>
    Это контейнер для изображения {{ imgUrl }}
    <img :src="imgUrl" alt="image">
    <ProseBlockquote>Жирная подпись</ProseBlockquote>
    <ContentSlot unwrap="button" :use="$slots.description" />
  </div>
</template>
