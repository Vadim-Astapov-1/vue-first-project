<script setup>
defineProps({
  class: {
    type: String,
    requared: true
  }
})
</script>

<template>
  <svg :class="class" width="30" height="25" viewBox="0 0 30 25" fill='none' xmlns="http://www.w3.org/2000/svg">
    <path
      d="M15.7031 5.46875L24.1406 12.5L15.7031 19.5312M22.9688 12.5H5.85938"
      fill="none"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
  </svg>
</template>
