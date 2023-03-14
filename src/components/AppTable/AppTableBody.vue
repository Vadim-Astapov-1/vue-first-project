<script setup></script>

<template>
  <div class="table__container">
    <slot></slot>
  </div>
</template>

<style scoped>
.table__container {
  max-width: 100%;
  min-height: 504px;
  display: flex;
  flex-direction: column;
}
</style>
