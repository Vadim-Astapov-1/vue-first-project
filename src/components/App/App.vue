<script setup>
  import TheNavbar from '../TheNavbar/TheNavbar.vue';
  import PageEmployee from '../PageEmployee/PageEmployee.vue';
</script>

<template>
  <div class='vue-settings-statistics'>
    <TheNavbar />
    <PageEmployee />
  </div>
</template>

<style scoped>
/* Fix - обнуление стилей Bitrix */
.workarea-content-paddings {
  padding: 0;
}

.vue-settings-statistics {
  width: 100%;
  display: grid;
  grid-template-columns: 305px 1fr;
  align-items: flex-start;
}
</style>