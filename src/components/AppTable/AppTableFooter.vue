<script setup>
import IconArrowLeft from '../Icons/IconArrowLeft.vue'
import IconArrowRight from '../Icons/IconArrowRight.vue'
</script>

<template>
  <div class="table__footer">
    <button type="button" class="table__btn-delete">Удалить выбранные</button>
    <div class="table__control">
      <button type="button" class="table__btn-change"><IconArrowLeft class='table__btn-change-icon' /></button>
      <p class="table__page-number">Страница 1</p>
      <button type="button" class="table__btn-change"><IconArrowRight class='table__btn-change-icon' /></button>
    </div>
    <p class="table__item-count">На странице:</p>
  </div>
</template>

<style scoped>
.table__footer {
  max-width: 100%;
  margin: 0 25px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.table__btn-delete {
  width: 184px;
  padding: 10px;
  background-color: #ffffff;
  border: 1px solid #545c6a;
  border-radius: 5px;
  color: #545c6a;
  transition: 0.3s;
  cursor: pointer;
}

.table__btn-delete:hover {
  background-color: #ff0000;
  color: #ffffff;
  border-color: #ff0000;
}

.table__control {
  max-width: 200px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.table__btn-change {
  width: 30px;
  height: 25px;
  border: 0;
  background-color: #ffffff;
  transition: 0.3s;
  cursor: pointer;
}

.table__btn-change-icon {
  stroke:#545c6a;
  fill: #545c6a;
}

.table__btn-change:hover .table__btn-change-icon {
  stroke: #1058D0;
  fill: #1058D0;
}
</style>
