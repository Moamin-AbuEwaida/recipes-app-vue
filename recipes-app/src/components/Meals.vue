<template>
  <div>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-3 p-8">
      <MealItem v-for="meal of meals" :key="meal.idMeal" :meal="meal" />
    </div>
    <div v-if="!meals.length" class="flex justify-center text-grey-600">
      There are no meals
    </div>
  </div>
</template>

<script setup>
import MealItem from "./MealItem.vue";
const { meals } = defineProps({
  meals: {
    require: true,
    type: Array,
  },
});
</script>

<style></style>
