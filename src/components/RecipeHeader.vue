<template>
  <div class="c-recipe-header">
    <img class="c-recipe-header__image" :src="imageSrc" :alt="title"  />
    <h1 class="c-recipe-header__title" v-text="title"></h1>
    <p class="c-recipe-header__description" v-text="description">
    </p>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title?: string;
  description?: string;
  imageSrc?: string;
}>();

</script>

<style scoped>
  .c-recipe-header__title {
    color: hsl(24, 5%, 18%);
  }

  .c-recipe-header__image {
    display: block;
    max-inline-size: 100%;
    inline-size: 100%;
    block-size: auto;
    border-radius: 8px;
  }
</style>