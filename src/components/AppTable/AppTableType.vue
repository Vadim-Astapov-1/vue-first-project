<script setup>
import AppTable from './AppTable.vue'
import AppTableCardEmployee from './AppTableCardEmployee.vue'
</script>

<template>
  <AppTable>
    <div class="table__heading"><AppTableCardEmployee /></div>
    <div class="table__container">
      <AppTableCardEmployee />
    </div>
  </AppTable>
</template>

<style scoped></style>
