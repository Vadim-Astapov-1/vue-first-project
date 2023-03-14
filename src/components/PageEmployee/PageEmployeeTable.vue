<script setup>
import AppTable from '../AppTable/AppTable.vue'
import AppTableHeading from '../AppTable/AppTableHeading.vue'
import PageEmployeeTableCard from './PageEmployeeTableCard.vue'
</script>

<template>
  <AppTable>
    <AppTableHeading>
      <input type="checkbox" class="table__checkbox" />
      <p class="table__text table__text_type_id">ID</p>
      <p class="table__text table__text_type_active">Активность</p>
      <p class="table__text table__text_type_type">Тип статистики</p>
      <p class="table__text table__text_type_date">Дата создания</p>
      <p class="table__text table__text_type_period">Периодичность</p>
      <p class="table__text table__text_type_employee">Сотрудник</p>
      <p class="table__text table__text_type_department">Подразделение</p>
    </AppTableHeading>
    <div class="table__container">
      <PageEmployeeTableCard />
    </div>
  </AppTable>
</template>

<style scoped>
.table__container {
  max-width: 100%;
  min-height: 460px;
  padding: 0 10px 0 25px;
  display: flex;
  flex-direction: column;
}
</style>
