<script setup>
import IconAdd from '../Icons/IconAdd.vue'
</script>

<template>
  <div class="table__header"> 
    <button type="button" class="table__header-btn-add"><IconAdd class='table__header-btn-icon' />Добавить</button>
    <p class="table__header-sum">Всего: 10</p>
  </div>
</template>

<style scoped>
.table__header {
  max-width: 100%;
  margin: 0 25px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: flex-end;
}

.table__header-btn-add {
  width: 129px;
  margin: 0;
  padding: 9px 10px 9px 44px;
  display: flex;
  flex-direction: row;
  border: 1px solid #58db84;
  border-radius: 5px;
  background-color: transparent;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #58db84;
  transition: 0.3s;
  cursor: pointer;
  position: relative;
}

.table__header-btn-add:hover {
  background-color: #58db84;
  color: #ffffff;
}

.table__header-btn-icon {
  position: absolute;
  top: 6px;
  left: 10px;
  transition: 0.3s;
  fill: #58db84;
}

.table__header-btn-add:hover .table__header-btn-icon {
  fill: #ffffff;
}
.table__header-sum {
  margin: 0;
  padding: 0;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #545c6a;
  text-align: right;
}
</style>
