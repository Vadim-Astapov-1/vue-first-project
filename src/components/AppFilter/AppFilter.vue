<script setup>

</script>

<template>
  <form class='filter'>
    <h2 class='filter__title'>Фильтр</h2>
    <div class='filter__container'>
      <slot></slot>
    </div>
    <div class='filter__btns'>
      <button type='submit' class='filter__btn'>Применить</button>
      <button type='button' class='filter__btn'>Сброс</button>
    </div>
  </form>
</template>

<style scoped>
.filter {
  width: 100%;
  display: flex;
  flex-direction: column;
  margin-left: 32px;
}

.filter__title {
  max-width: 250px;
  padding: 15px 0;
  margin: 0;
  border-bottom: 1px solid #545C6A;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #4A4747;
  cursor: default;
}

.filter__container {
  width: 100%;
  margin-top: 17px;
  display: grid;
  grid-template-columns: repeat(auto-fill, 250px);
  gap: 10px 30px;
}

.filter__btns {
  max-width: 520px;
  margin-top: 20px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.filter__btn {
  width: 250px;
  padding: 10px 15px;
  border: 1px solid #545C6A;
  border-radius: 5px;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #545C6A;
  background-color: transparent;
  transition: 0.3s;
  cursor: pointer;
}

.filter__btn:hover {
  background-color: #545C6A;
  color: #ffffff;
}
</style>
