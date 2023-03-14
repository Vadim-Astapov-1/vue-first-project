<script setup>
import IconArrowLeft from '../Icons/IconArrowLeft.vue'
import IconArrowRight from '../Icons/IconArrowRight.vue'
</script>

<template>
  <div class="table__footer">
    <button type="button" class="table__btn-delete">Удалить выбранные</button>
    <div class="table__control">
      <button type="button" class="table__btn-change"><IconArrowLeft /></button>
      <p class="table__page-number">Страница 1</p>
      <button type="button" class="table__btn-change"><IconArrowRight /></button>
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
  min-width: 200px;
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
  stroke: #545c6a;
}

.table__btn-change:hover {
  stroke: #1058d0;
}

.table__page-number {
  max-width: 100%;
  margin: auto 10px;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #545c6a;
  cursor: default;
}

.table__item-count {
  max-width: 115px;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #545c6a;
  text-align: right;
}
</style>
