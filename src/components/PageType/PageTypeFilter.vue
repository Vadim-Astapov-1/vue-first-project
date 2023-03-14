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

<style scoped></style>
