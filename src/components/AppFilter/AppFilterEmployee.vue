<script setup>
import AppFilter from './AppFilter.vue';
import AppSearchInputUsers from '../AppSearchInput/AppSearchInputUsers.vue';
</script>

<template>
  <AppFilter>
    <div class='filter-search'>
      <label class='filter-search__title'>Поиск</label>
      <AppSearchInputUsers />
    </div>
  </AppFilter>
</template>

<style scoped>
.filter-search {
  width: 100%;
  display: flex;
  flex-direction: column;
}

.filter-search__title {
  width: 100%;
  margin-bottom: 10px;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  line-height: 17px;
  color: #545C6A;
}
</style>
