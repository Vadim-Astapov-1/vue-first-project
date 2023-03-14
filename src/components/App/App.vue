<script setup>
import { ref } from 'vue'

import TheNavbar from '../TheNavbar/TheNavbar.vue'
import PageEmployee from '../PageEmployee/PageEmployee.vue'
import PageType from '../PageType/PageType.vue';

const isFirstPage = ref(true);

const handleChangePage = () => {
  isFirstPage.value = !isFirstPage.value;
}
</script>

<template>
  <div class="vue-settings-statistics">
    <TheNavbar :isFirstPage="isFirstPage" @changePage="handleChangePage" />
    <PageEmployee v-if="isFirstPage" />
    <PageType v-else />
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
