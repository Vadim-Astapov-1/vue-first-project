<script setup>
import AppTable from '../AppTable/AppTable.vue'
import AppTableBody from '../AppTable/AppTableBody.vue'
import AppTableHeading from '../AppTable/AppTableHeading.vue'
import PageTypeTableCardVue from './PageTypeTableCard.vue'
</script>

<template>
  <AppTable>
    <AppTableBody>
      <AppTableHeading>
        <input type="checkbox" class="table__checkbox" />
        <p class="table__text table__text_type_id">ID</p>
        <p class="table__text table__text_type_active">Активность</p>
        <p class="table__text table__text_type_name">Название</p>
        <p class="table__text table__text_type_date">Дата создания</p>
        <p class="table__text table__text_type_scored">Балльная статистика</p>
        <p class="table__text table__text_type_point">Количество баллов</p>
        <p class="table__text table__text_type_related">Связанные типы статистик</p>
        <p class="table__text table__text_type_related-sum">Суммировать связанные типы статистик</p>
      </AppTableHeading>
      <PageTypeTableCardVue />
    </AppTableBody>
  </AppTable>
</template>

<style scoped></style>
