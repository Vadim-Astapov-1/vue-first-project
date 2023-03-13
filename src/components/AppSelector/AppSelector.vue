<script setup></script>

<template>
  <div class="select-box">
    <label class="select-box__label">Заголовок</label>
    <div class="select-box__input-container">
      <input type="text" class="select-box__input" readonly />
      <div class="select-box__results">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<style scoped>
.select-box {
  max-width: 100%;
  max-height: 25px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.select-box__label {
  max-width: 125px;
  margin: 0;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  line-height: 17px;
  color: #545c6a;
}

.select-box__input-container {
  max-width: 100%;
  position: relative;
}

.select-box__input {
  max-width: 104px;
  padding: 5px 10px;
  border: 1px solid #545c6a;
  border-radius: 5px;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 13px;
  line-height: 15px;
  color: #1058d0;
  outline: none;
  cursor: pointer;
}

.select-box__results {
  width: 100%;
  position: absolute;
  top: 35px;
  left: 0;
  display: flex;
  flex-direction: column;
  box-shadow: 0px 0px 6px 4px rgba(212, 212, 212, 0.25);
  background-color: #ffffff;
}
</style>
