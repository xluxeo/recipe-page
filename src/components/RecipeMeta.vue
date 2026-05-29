<template>
  <div class="c-recipe-meta">
    <h2 class="c-recipe-meta__title" v-text="title"></h2>
    <ul class="c-recipe-meta__list">
      <li class="c-recipe-meta__item" v-for="(item, index) in metaItems" :key="index" v-text="item"></li>
    </ul>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title?: string;
  metaItems?: string [];
}>();

</script>


<style scoped>
  .c-recipe-meta {
    border-radius: 12px;
    padding: 12px;
    background-color: hsl(330, 100%, 98%);
  }

  .c-recipe-meta__title {
    padding-inline-start: 18px;
    color: hsl(332, 51%, 32%);
    font-size: 1rem;
    font-weight: 700;
    font-family: 'Outfit', sans-serif;
  }

  .c-recipe-meta__item::marker {
    padding-block-end: 8px;
    color: hsl(332, 51%, 32%);
  }

  .c-recipe-meta__item {
    padding-block-end: 8px;
  }
</style>

