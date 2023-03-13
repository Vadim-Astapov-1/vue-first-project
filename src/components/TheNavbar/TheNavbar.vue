<script setup></script>

<template>
  <div class="navbar">
    <div class="navbar__container">
      <h2 class="navbar__title">Отображение</h2>
      <div class="navbar__btn-container">
        <button type='button' class="navbar__btn navbar__btn_active">Статистика сотрудников</button>
        <div class="navbar__btn-background"></div>
      </div>
      <div class="navbar__btn-container">
        <button type='button' class="navbar__btn">Типы статистики</button>
        <div class="navbar__btn-background"></div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.navbar {
  width: 250px;
  padding: 0 30px 52px 25px;
  display: block;
  border-right: 1px solid #545C6A;
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
  border-bottom: 1px solid #545C6A;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #4A4747;
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
  color: #545C6A;
  text-align: left;
  transition: 0.3s;
  cursor: pointer;
  z-index: 1;
}

.navbar__btn:hover {
  color: #1058D0;
}

.navbar__btn:hover+.navbar__btn-background {
  border-left: 1px solid #1058D0;
  border-bottom: 1px solid #1058D0;
}

.navbar__btn_active {
  color: #1058D0;
}

.navbar__btn_active+.navbar__btn-background {
  width: 200px;
  border-left: 1px solid #1058D0;
  border-bottom: 1px solid #1058D0;
}

.navbar__btn-background {
  width: 125px;
  height: 16px;
  box-sizing: content-box;
  border-left: 1px solid #545C6A;
  border-bottom: 1px solid #545C6A;
  position: absolute;
  bottom: 0;
  left: 0;
}
</style>
