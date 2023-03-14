<script setup>
import AppTable from '../AppTable/AppTable.vue'
import AppTableBody from '../AppTable/AppTableBody.vue'
import AppTableHeading from '../AppTable/AppTableHeading.vue'
import PageEmployeeTableCard from './PageEmployeeTableCard.vue'
</script>

<template>
  <AppTable>
    <AppTableBody>
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
      <PageEmployeeTableCard />
    </AppTableBody>
  </AppTable>
</template>

<style scoped></style>
