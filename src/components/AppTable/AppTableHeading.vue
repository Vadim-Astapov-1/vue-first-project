<script setup></script>

<template>
  <div class="table__heading">
    <slot></slot>
  </div>
</template>

<style scoped>
.table__heading {
  max-width: 100%;
  margin-top: 5px;
  padding: 0 25px;
  display: inline-flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  border-bottom: 2px solid #ebf0f5;
}

:slotted(.table__checkbox) {
  width: 22px;
  height: 22px;
  box-sizing: border-box;
  border: 1px solid #000000;
  border-radius: 5px;
  position: relative;
  cursor: pointer;
  appearance: none;
  outline: none;
}

:slotted(.table__checkbox::before) {
  content: '';
  position: absolute;
  top: 3px;
  left: 3px;
  width: 14px;
  height: 14px;
  background-color: transparent;
  border-radius: 3px;
  transition: 0.3s;
}

:slotted(.table__checkbox:checked::before) {
  background-color: #00ff57;
}

:slotted(.table__text) {
  max-width: 100%;
  width: 100%;
  margin: 0 0 0 25px;
  padding: 14px 0;
  font-family: 'Segoe UI';
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 16px;
  color: #000000;
  cursor: default;
}

:slotted(.table__text_type_id) {
  max-width: 55px;
}

:slotted(.table__text_type_active) {
  max-width: 90px;
}

:slotted(.table__text_type_type) {
  max-width: 120px;
}

:slotted(.table__text_type_date) {
  max-width: 120px;
}

:slotted(.table__text_type_period) {
  max-width: 120px;
}

:slotted(.table__text_type_employee) {
  max-width: 220px;
}

:slotted(.table__text_type_department) {
  max-width: 220px;
}

:slotted(.table__text_type_name) {
  max-width: 200px;
}

:slotted(.table__text_type_scored) {
  max-width: 140px;
}

:slotted(.table__text_type_point) {
  max-width: 135;
}

:slotted(.table__text_type_related) {
  max-width: 200px;
}

:slotted(.table__text_type_related-sum) {
  max-width: 274px;
}
</style>
