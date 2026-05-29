<template>
  <div class="c-instructions-list">
    <h2 class="c-instructions-list-title" v-text="title"></h2>
    <ol class="c-instructions-list-items">
      <li class="c-instructions-list-item" v-for="(item, index) in items" :key="index" v-text="item"></li>
    </ol>
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