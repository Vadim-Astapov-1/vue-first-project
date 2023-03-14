<script setup>
import AppFilter from '../AppFilter/AppFilter.vue'
import AppSearchInputTypeStatistics from '../AppSearchInput/AppSearchInputTypeStatistics.vue'
import AppSelectorActive from '../AppSelector/AppSelectorActive.vue'
import AppSelectorScored from '../AppSelector/AppSelectorScored.vue'
import AppSelectorCalender from '../AppSelector/AppSelectorCalender.vue'
</script>

<template>
  <AppFilter>
    <div class="filter__container">
      <label class="filter__container-title">Поиск</label>
      <AppSearchInputTypeStatistics />
    </div>
    <div class="filter__container">
      <AppSelectorActive />
      <AppSelectorScored />
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
