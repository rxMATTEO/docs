<template>
  <div :class="$style.container" class="123">
    <slot />
  </div>
</template>

<script setup lang="ts">

</script>

<style module>
.container {
  padding: 0 168px;
}
</style>