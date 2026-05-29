<template>
  <div class="c-nutrition-table">
    <h2 class="c-nutrition-table__title" v-text="title"></h2>
    <p class="c-nutrition-table__text" v-text="text"></p>
    <table class="c-nutrition-table__table">
      <tbody>
        <tr>
          <td>Calories</td>
          <td>277 kcal</td>
        </tr>
        <tr>
          <td>Carbs</td>
          <td>0 g</td>
        </tr>
        <tr>
          <td>Protein</td>
          <td>20 g</td>
        </tr>
        <tr>
          <td>Fat</td>
          <td>22 g</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title?: string;
  text?: string;
}>();
</script>

<style scoped>
</style>

