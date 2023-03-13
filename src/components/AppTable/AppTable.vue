<script setup>
import AppTableHeader from './AppTableHeader.vue'
import AppTableFooter from './AppTableFooter.vue'
</script>

<template>
  <div class='table'>
    <AppTableHeader />
    <slot></slot>
    <AppTableFooter />
  </div>
</template>

<style scoped>
.table {
  max-width: 100%;
  margin-top: 15px;
  margin-bottom: 25px;
  display: flex;
  flex-direction: column;
  grid-column: 1/3;
}
</style>
