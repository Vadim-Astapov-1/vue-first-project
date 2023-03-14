<script setup>
defineProps(['isFirstPage'])
defineEmits(['changePage'])
</script>

<template>
  <div class="navbar">
    <div class="navbar__container">
      <h2 class="navbar__title">Отображение</h2>
      <div class="navbar__btn-container">
        <button type="button" class="navbar__btn" :class="{ navbar__btn_active: isFirstPage }" @click="$emit('changePage')">
          Статистика сотрудников
        </button>
        <div class="navbar__btn-background"></div>
      </div>
      <div class="navbar__btn-container">
        <button type="button" class="navbar__btn" :class="{ navbar__btn_active: !isFirstPage }" @click="$emit('changePage')">
          Типы статистики
        </button>
        <div class="navbar__btn-background"></div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.navbar {
  width: 250px;
  min-height: 220px;
  padding: 0 30px 0 25px;
  display: block;
  border-right: 1px solid #545c6a;
}

.navbar__container {
  width: 100%;
  display: flex;
  flex-direction: column;
}

.navbar__title {
  max-width: 100%;
  margin: 0 0 10px 0;
  padding: 15px 0;
  border-bottom: 1px solid #545c6a;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #4a4747;
  cursor: default;
}

.navbar__btn-container {
  width: 100%;
  display: block;
  position: relative;
}

.navbar__btn {
  width: 100%;
  padding: 15px 0 15px 10px;
  border: 0;
  position: relative;
  background-color: transparent;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 18px;
  color: #545c6a;
  text-align: left;
  transition: 0.3s;
  cursor: pointer;
  z-index: 1;
}

.navbar__btn:hover {
  color: #1058d0;
}

.navbar__btn-background {
  width: 125px;
  height: 16px;
  box-sizing: content-box;
  border-left: 1px solid #545c6a;
  border-bottom: 1px solid #545c6a;
  position: absolute;
  bottom: 0;
  left: 0;
  transition: 0.3s;
}

.navbar__btn:hover + .navbar__btn-background {
  border-left: 1px solid #1058d0;
  border-bottom: 1px solid #1058d0;
}

.navbar__btn_active {
  color: #1058d0;
}

.navbar__btn_active + .navbar__btn-background {
  width: 200px;
  border-left: 1px solid #1058d0;
  border-bottom: 1px solid #1058d0;
}
</style>
