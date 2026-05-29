<template>
  <div class="c-ingredients-list">
    <h2 class="c-ingredients-list-title" v-text="title"></h2>
    <ul class="c-ingredients-list-items">
      <li class="c-ingredients-list-item" v-for="(item, index) in items" :key="index" v-text="item"></li>
    </ul>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title?: string;
  items?: string [];
}>();

</script>

<style scoped>
</style>