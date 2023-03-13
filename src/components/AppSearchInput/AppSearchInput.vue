<script setup></script>

<template>
  <div class="search-box">
    <input type="text" class="search-box__input" placeholder='что-то' />
    <div class="search-box__btn-container">
      <button type="button" class="search-box__btn search-box__btn_active">Имя сотрудника</button>
      <button type="button" class="search-box__btn">ID</button>
    </div>
    <div class="search-box__result-container">
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>
.search-box {
  max-width: 100%;
  display: grid;
  grid-template-columns: 1fr;
  gap: 10px 0;
  position: relative;
}

.search-box__input {
  width: 100%;
  padding: 0 0 5px 0;
  border: 0;
  border-bottom: 1px solid #545c6a;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 13px;
  line-height: 15px;
  color: #1058d0;
  outline: none;
}

.search-box__btn-container {
  max-width: 100%;
  display: flex;
  flex-direction: row;
}

.search-box__btn {
  padding: 5px 10px;
  border: 1px solid #545c6a;
  border-radius: 5px;
  background-color: #ffffff;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 12px;
  line-height: 14px;
  color: #545c6a;
  transition: 0.3s;
  cursor: pointer;
}

.search-box__btn:first-of-type {
  margin-right: 10px;
}

.search-box__btn:hover {
  border: 1px solid #1058d0;
  color: #1058d0;
}

.search-box__btn_active {
  border: 1px solid #1058d0;
  color: #1058d0;
}

.search-box__result-container {
  width: 100%;
  position: absolute;
  top: 30px;
  left: 0;
  background-color: #ffffff;
}
</style>
