<script setup>
import AppFilter from '../AppFilter/AppFilter.vue'
import AppSearchInputUsers from '../AppSearchInput/AppSearchInputUsers.vue'
import AppSelectorActive from '../AppSelector/AppSelectorActive.vue'
import AppSelectorPeriod from '../AppSelector/AppSelectorPeriod.vue'
import AppSelectorCalender from '../AppSelector/AppSelectorCalender.vue'
</script>

<template>
  <AppFilter>
    <div class="filter__container">
      <label class="filter__container-title">Поиск</label>
      <AppSearchInputUsers />
    </div>
    <div class="filter__container">
      <AppSelectorActive />
      <AppSelectorPeriod />
    </div>
    <div class="filter__container">
      <AppSelectorCalender />
      <AppSelectorCalender />
    </div>
  </AppFilter>
</template>

<style scoped>
.filter__container {
  width: 100%;
  display: grid;
  grid-template-columns: 1fr;
  gap: 10px 0;
}

.filter__container-title {
  width: 100%;
  margin-bottom: 10px;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  line-height: 17px;
  color: #545c6a;
}
</style>
