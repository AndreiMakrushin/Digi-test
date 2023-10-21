<script setup>
import CategoryFilter from "./sidebar-conponents/category-filter/CategoryFilter.vue";
import PriceFilter from "./sidebar-conponents/category-filter/PriceFilter.vue";
import CheckboxFilter from './sidebar-conponents/category-filter/CheckboxFilter.vue';
import SizeFilter from "./sidebar-conponents/category-filter/SizeFilter.vue";
</script>
<template>
  <div class="sidebar-container">
    <CategoryFilter />
    <PriceFilter />
    <CheckboxFilter />
    <SizeFilter />
  </div>
</template>
<style scoped>
.sidebar-container {
  display: flex;
  flex-direction: column;
}
</style>
